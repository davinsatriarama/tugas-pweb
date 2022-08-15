-- phpMyAdmin SQL Dump
-- version 5.1.1
-- https://www.phpmyadmin.net/
--
-- Host: 127.0.0.1
-- Generation Time: Aug 09, 2022 at 05:59 AM
-- Server version: 10.4.21-MariaDB
-- PHP Version: 7.4.25

SET SQL_MODE = "NO_AUTO_VALUE_ON_ZERO";
START TRANSACTION;
SET time_zone = "+00:00";


/*!40101 SET @OLD_CHARACTER_SET_CLIENT=@@CHARACTER_SET_CLIENT */;
/*!40101 SET @OLD_CHARACTER_SET_RESULTS=@@CHARACTER_SET_RESULTS */;
/*!40101 SET @OLD_COLLATION_CONNECTION=@@COLLATION_CONNECTION */;
/*!40101 SET NAMES utf8mb4 */;

--
-- Database: `db_02_08`
--

-- --------------------------------------------------------

--
-- Table structure for table `tb_biodatasaya`
--

CREATE TABLE `tb_biodatasaya` (
  `id` int(11) NOT NULL,
  `nama` varchar(100) NOT NULL,
  `alamat` varchar(100) NOT NULL,
  `jenis kelamin` enum('laki laki','perempuan') NOT NULL,
  `nomor hp` int(13) NOT NULL
) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4;

--
-- Dumping data for table `tb_biodatasaya`
--

INSERT INTO `tb_biodatasaya` (`id`, `nama`, `alamat`, `jenis kelamin`, `nomor hp`) VALUES
(1, 'affan prayogi', 'jl. camat kuswari rt05 rw01 tegalsari, kepanjen, malang 65163', 'laki laki', 10000000),
(2, 'davin satria rama', 'jln probolinggo rt02 rw02 penarukan, kepanjen, malang 65163', 'laki laki', 20000000),
(3, 'gatra rahayu', 'jl.blimbing', 'laki laki', 10000000),
(4, 'coirul', 'jln sambigede', 'laki laki', 20000000),
(5, 'syafii', 'sukorahajo', 'laki laki', 50000000),
(6, 'aaaa', 'aaaaaaaaaaaaaaaa', 'laki laki', 12345);

--
-- Indexes for dumped tables
--

--
-- Indexes for table `tb_biodatasaya`
--
ALTER TABLE `tb_biodatasaya`
  ADD PRIMARY KEY (`id`);

--
-- AUTO_INCREMENT for dumped tables
--

--
-- AUTO_INCREMENT for table `tb_biodatasaya`
--
ALTER TABLE `tb_biodatasaya`
  MODIFY `id` int(11) NOT NULL AUTO_INCREMENT, AUTO_INCREMENT=8;
COMMIT;

/*!40101 SET CHARACTER_SET_CLIENT=@OLD_CHARACTER_SET_CLIENT */;
/*!40101 SET CHARACTER_SET_RESULTS=@OLD_CHARACTER_SET_RESULTS */;
/*!40101 SET COLLATION_CONNECTION=@OLD_COLLATION_CONNECTION */;
