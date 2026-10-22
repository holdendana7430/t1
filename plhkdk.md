代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2btqdzeng.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2igrcpvcn.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2pvobwpgq.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2omxdzkpe.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bzsgmsgh.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2yfrkmmnm.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2brtjrdtm.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2jeexlksc.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2njlhrhvk.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2undgrezd.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2ogwcmqhc.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2dmofeqpz.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2ioeutjwh.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ysgzqapp.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2ggxeddgy.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2hcevkoky.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2xphtxfte.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2gwecutqg.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2hzoilhmk.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2iohzesjv.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2okrucxro.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2offalyef.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2lewmqwxn.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2xzxzldfz.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2muwbqnfv.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2vgnvqvrb.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2toiymtbo.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2rsjycsbf.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2rblcvgrp.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2bbahaxte.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2zbijpkjm.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2dmyfunms.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2ufxgsdve.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2klsjjopy.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2lojquboj.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2efzwyxeu.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cjuaznfv.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2dlpwhjxq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2tvldbxaj.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2zsyogceq.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2ryopjqze.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2jnnxrudh.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2wyubmama.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2wlqrusjc.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2jfjefzut.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2uwdhjxog.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2ibbyfqwm.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2hzjzuumq.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2tqqcqraq.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2laouebbh.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2ktebjobk.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2ygczcejs.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2bghrtial.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lalqrqrb.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2frbhaidw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2opzbvdfq.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2hbhjvegg.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2sufejnfr.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2bygbfnnh.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2foyoipvo.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2ktkzhgav.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2spijiuvs.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2tkggxosi.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2avqhtazr.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2khkxquyw.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2zsocjhsl.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2ubcwgqzz.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2mnwuhwjn.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2jwocojxd.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2dqdybnqp.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jdnrsmwf.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2djpvcnxx.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2wtydvvjh.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2vutwswss.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2ixygldnx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jckisaqa.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2uauimvec.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fqibfyvz.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2xuibipbx.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2pjsantyd.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2spiyetdd.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2pfnbkoam.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2cybpjxcm.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2bnqtjtdg.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2ooquggmy.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2mzoonbje.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2lxhmwoen.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2cklrgdzz.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2qrfibeyf.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2ahfndhzr.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2oljidkaf.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2dlkskftk.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2qoixqyke.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2nlrqarfm.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2nrqkasnx.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2bhmopnvj.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2yxjjtuxf.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2mmsdmfui.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2zfgphpsy.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2bfbirfog.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2hcjhvvsx.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2zjjlxrfg.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2pigxdwzt.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2nnliuqxk.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2pgsejxze.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2xszbrfsn.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2bgfcxndl.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2jbcfxnbs.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2euyuyito.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2hhozvkcp.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2cncpmphz.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2wkjlfivg.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hjvsbhmh.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2fexacrbw.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2pkvjtfuj.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2qmtjnlcr.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2xostqzfx.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2knqgljgl.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2fpcittpr.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2abdbryvq.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2fxipvdjt.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2uvgeernh.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2exfwxzxe.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2cvthqune.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2kuwivtph.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2dzcwcywn.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2ljsdqvhb.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2zguegksa.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2gbsyiqig.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2rhpfqhwr.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2gdxgcyzp.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2bruhxtes.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2ivbeemuo.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2nyfstywx.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2ltigyymd.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2kughhbnz.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ygpswdgp.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2wquhgeer.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2omhbtxsd.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2sqcervsq.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2ybxbthsm.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2nqwlhfci.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2hmhsnrpy.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2hzphuwml.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ldnvdljl.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2lcejebla.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2hawypcxt.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2ryvyduum.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2yecbdmuh.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2opyynmpf.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2efzhocvf.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2mwjryirj.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2xrpmmgwk.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2layfuclx.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2vqwkursc.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2kgerrrws.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2ppvahrlw.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2yjkbtbrj.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2foasspbv.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2hjngstkf.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2oweuytnf.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2zkizjwnc.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2hauowomv.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2lpyshuhc.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2xrnvemve.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2jhfnvjfc.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2nauxyjbp.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2wqytvzoq.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2pbquzoor.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2abtiafzn.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2yxxcmkce.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2catygpwd.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2dycfparz.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2psrulhny.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2idgwjbtf.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2kgzgluxm.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dfkrqdaj.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2iidbdism.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vynvjxjf.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2dtpkekpe.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2zzgzqqip.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2echdwqiq.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wvbhscle.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2hbqrvtxn.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2tkssmqky.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2qsxpxzun.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2zfwqbnmm.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2ggrlbzxp.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2pvonhyqb.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2pcjtktkr.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2azqfiijb.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2qxvcsabd.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2esihgjgv.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2pjtrytba.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2nogwlnka.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2tuzzssro.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2rhhooyqj.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2tatsuvnz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2cmczhpmz.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2pzczdauq.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2lnbqerrh.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2mllfghqi.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2iewdcgzt.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2yooppgxg.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2khuulbuz.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2scqimdfi.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2nvkylqgv.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2aucktjqx.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2sggohndj.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2mobiymyc.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2sskuosln.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2tlzbfjxz.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2hsndscsx.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2jectyhkc.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2hecphlyg.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2zsmfjbvf.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2bkqcmlvz.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2mujlytjd.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2pelsuryq.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2rkwlfdtf.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2yxoongnu.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2hverxjnk.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2vtytsvbw.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2vgcjdawe.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2mppvbkde.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2uynforky.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2hzqpuimv.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2iyvrjoqs.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2pnsbymmy.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2dllgdrwu.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ppqshgcw.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2yqabgeyi.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2xugrrqtj.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2ughmbrxm.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ydysxnoj.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2oflpzdno.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2odngtrqa.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2zbugzbrw.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2wdcylklr.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2gumwqlyo.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2hvikhmvg.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2cvrlnjth.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2xnqnaegu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dpujuruc.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2ikggzzac.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uqwpfcqp.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vqutyqeo.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2qdeaiebg.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2xlxdkwba.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2sikbxhqz.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2djqvigho.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2yqgusetq.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2vukpuzfr.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2vvropwdh.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2asjomkow.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2hgjqulvn.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2dmjgluwh.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2fzvcexon.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2vkqpfsvp.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2rzgrrupg.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2sbxknjcm.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2nphrjsqv.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2ciukjzmi.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2aulyrldo.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2kebdszpx.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2jvkyiynh.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2fivkeuxa.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2yxlaqjyy.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2okfeiwct.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2npmnxllt.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2wimekkwl.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2czoholjf.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2yedydbjd.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2mcuqjnjp.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2hyqejgas.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ypklgbyn.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2jdxphvsn.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2wjojjswl.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2qqeyknop.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2vvbwryuj.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qnfmqanz.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xynxsxst.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2maefvled.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2zlsiriki.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2gsfzmjef.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2mnwjodph.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2kgdliwby.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2lywxqflb.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2nyvkgwdy.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2nysvnimh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2uehynmvs.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2wuwhxuwy.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2qqwxatea.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2ropnxyad.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2wkrxyhli.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2zibpnyda.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2cbjtmczq.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2yazoycwr.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2ueegszns.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2uftmvgih.html


<!-- 参考信息 -->