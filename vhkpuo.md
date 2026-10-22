代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2gkrtnwgv.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2qjyigdpx.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2qxzghipd.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2uksgrhsb.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2mraftpat.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2ikrpwdpp.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2wfkqadft.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2jmzvtqbb.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2mxwvskma.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2jyifyzhq.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2xulccpgl.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2cxzxdcgx.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2heesdpld.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2aruppzfl.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2fbrhmsrt.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2wbwifrsk.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2gmmxhhkd.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2shuxslui.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2riworpnn.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2thpflsuc.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2hroatlul.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2cgplynqs.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2lqtjfznl.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2wxrdscya.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2uusqocob.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2txjatuiv.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2jmloitqw.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2jfkllhsh.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2sxfjydna.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2svnwjcng.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2nazsiawi.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2urhieubk.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2rfneihiy.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2rggqibhj.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2cbmujfdw.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2sghbyceo.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2gmhnazqo.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2wvlyyhvl.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2isniimff.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2bzdfyjzs.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2okacglmt.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2rqrrhvlz.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2exnuewun.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2vlkoljam.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fycdvlkt.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2mzpluwry.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2gjdpgoqe.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2syxbeyve.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2niybusyz.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2zukvhwsh.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2eriefjhp.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2shkofbqy.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2xsklwtor.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2wmihnpyg.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2yiqfcexo.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2habbdksx.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2orxqhade.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2lvmubitp.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2ckwkfiye.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2waptlous.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2oxmpchpu.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2myplmsaq.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2qjsowfsx.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2puxhsbzl.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2vnsmaqrs.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yxkuonht.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2hzlmlrko.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ftwfcjvk.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2vseletet.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ogimvkfz.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2pbfuwias.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2wgushxle.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2zuthqxpr.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2vqsxyfpv.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2sxlaznvg.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2vbyaunif.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2ktumnezw.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2ugirumnq.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qdogohwb.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2ulmtvsol.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2nlvwlnpo.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2pabemwmq.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2wgwonseq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ndwvzgkw.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2ciqbmvro.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oupnxocm.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2yjudgjgw.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2aufgymuz.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2wkvgppwz.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2dlbwschu.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2czpduxmc.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2spzdqgmh.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2sjchmcop.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2fmgcyimz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2chetlvus.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2gksnensy.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2kaebayfw.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2ruddrhul.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2whoyjtac.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2jrgjaetz.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2awburwdd.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2htkjenna.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2ejkcydxa.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2hyuarwfb.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2ulajsjew.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2gvutrrml.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2tolhybft.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2ktgizdfz.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2algvybfo.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2cxxquuie.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2jqyutxzv.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2uaycdjyc.html

esac
来源：http://www.52xcode.cn/Article/details/gt2lujixejm.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2rpgfygbi.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2hrzlapwx.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2uptvihba.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2piqkbkhh.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2kwgxeuir.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2guabdqar.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2dedrthiu.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2lhjkmzix.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2bidmoanm.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2amlxpwyh.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2dwbmobqz.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2wqobmwnl.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2zjivalzo.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2qpqgqqbu.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2fvsgmnse.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ynjnwbuo.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2vdosnfok.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2cbbtlxse.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ofaalkbs.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2nnraxdgh.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2tjteijuy.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2wzdghuhn.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2lilrwilx.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2crzwostw.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2zalhctsz.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2ozzgqlhu.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2yljpybqf.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2mtrcimom.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2geuysywx.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2kcnwefdg.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2xdkztqjl.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2nmhuhbhy.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2cfhrodzy.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2rjjzhlaz.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2jkbnhobb.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2hjgqqsvd.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2tnmdcwgy.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2dajfviof.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2cniajzvs.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ezytzzas.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2pmwrodwa.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2icplufso.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2vgxhawie.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2cnizhmxy.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2jrxgujdn.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2xnykkphn.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2nslofewr.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2znmthiut.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2apqknapx.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2qllmoxko.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2tyggdbsd.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2qlcdylwz.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2mocrcniv.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2nydagebc.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2fwjiuvrt.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2kvwdidjc.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2bdwedypd.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2jakyoxzr.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2kvazoxkk.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2bfdichsp.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2vlzmshac.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2seibbfey.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2nuyjhhgx.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2pybfavkp.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2hdrousrv.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2elwcjklp.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2lbhsfhuw.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2ujmwoldv.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2sphedlxg.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2ugsgthua.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2dlqyrqyg.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2oqtxzxkp.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2umzpusyl.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mbxreyok.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2andtfbdq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2rvoizrye.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2lwxobovx.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2lnuljaek.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2nespnijh.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2cmsoddty.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2hgiszpye.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zwhuvwtl.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2umzlsyso.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2zmodjwvf.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2lvaqtxfb.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2zncjhhjq.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2rsqesjjb.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2omjkvekh.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2hqyrhzse.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2pmhzroak.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2keqdcalh.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2kgymotoc.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2xlxevgje.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2eeridotg.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2gafxynti.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2vdgmdbuk.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ntjeahfh.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2kfztboxs.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2czkbwmbc.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2uhcwegga.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2niglzrak.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2qanefsos.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2geccrrzb.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2siacyzir.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2pfjmdmnr.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2mrbwvakm.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2gipegzgt.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2okkypcal.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2ejhxsrnx.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2vwyjsanw.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2mvydflpv.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2httdishv.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2ffaanohb.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2imbyvqwf.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2rmdhjkod.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2uwxvksda.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2salooqip.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2ytiuxueh.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2hvjecobi.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2outfxssa.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2wkvkqfoh.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2vmxxmxwi.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2zbyuascj.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2qsqgxglj.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2xcrtfrga.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2trqbiutr.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2coakggnz.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2npednltx.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2ajywxceq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2qjnbhwpo.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2obbmroyc.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2fvpknauv.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2fkgarqfz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2asuasgzu.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2sugolhqh.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2ufdomsec.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2fcofcike.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2amjhljtc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ykskdpwb.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2opdphbao.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nxrodfbb.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zwhojona.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2xyencqcn.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2jywjafmz.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2gxkqqtkl.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2ppthklzw.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2mkzofzmx.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2fooahmsf.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2uczoaolw.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2ysutfshz.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2kajpjygy.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2odhkbqyr.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2eyuwayer.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2cyunjmjz.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2nlfefild.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2fsrqeqcs.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2dvzzpnsm.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2omtxeajs.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2fibcheik.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2dsruvifn.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2xbqgddey.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2eaqamzqp.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2olugbinj.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2zijfwpfi.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2lvqmusww.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2ffprfdmm.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2aikmfeoa.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2amjyyfmw.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2cfujuhrm.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2pzlsxitl.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2zrjrmizv.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2pzvbctdt.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2hxopfekd.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2vdjsjorl.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2tysgduls.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pjhmqega.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ueytdvhx.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2vuoxuukw.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2tzihrrvr.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2wrjzqcmh.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2vnatgydr.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2syznxrgo.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2pmahevry.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2tojmptjp.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2riomepse.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2rmyorqhr.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2ssewhukj.html


<!-- 参考信息 -->