代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2pprgidne.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2fmlfrqtl.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2indypbfz.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2jyipwwmu.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2tctszwts.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2hxkttxif.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2aluhyafr.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2iiofjovb.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2osaucwqe.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2fosnfrzn.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2dwyywymn.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2wxlynuyk.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2blnnnwtu.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2jpoyhnhf.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2gyldizch.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2dvheeccf.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2emswnzfn.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2ngdcchpf.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2vqwoismz.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2atjbhxmn.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2kpdubhet.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2nkugjeig.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2uvhjnqnk.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2bgpgimpt.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2dsjecdbn.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2evvpkrpy.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2fkphpbpn.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2gygmkfhz.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2zcohpvav.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2pgthbbur.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2aowdwcwb.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2gpelnlfa.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2ocplkuzc.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2irobilrl.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2jkqfkkzy.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2tlgfzito.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2psqxtjfe.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2mrjxrtpf.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2ilzxankt.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2ppncakaq.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2rrnvdjdd.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2rolexwlx.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2ekjhfueq.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2syihljtk.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2yefnfzqo.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2rgywrldv.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2iuibsfex.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2cpeoignb.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uxiawied.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2wlzcrnkz.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2lmbajnxn.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2vifjxanx.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2ufknnwbw.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2esfvcubv.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2popymnrl.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2thvrqhgc.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2xlixeezu.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2jhwlacri.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2uahqsmna.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2jxiihzub.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2xyylhtro.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2kzkgrjuy.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2swppheyl.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2btroipwd.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2ggjxqhss.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ccoysicv.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2gozcibpi.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mzhqsgbi.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2ljquefmh.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zajbaqoq.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2xsblzaaz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cxhkjwmm.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2arevoemh.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rwvnebfr.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2ykqskxcc.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2muwmiixn.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2hombcitm.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2vpetaoqd.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2yreccdts.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2vjqmwxtj.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2pgcqtxud.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2syreffsa.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jtqgzdnd.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2ttzyckhf.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2lviwlvmi.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2oernitec.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2bhrzyobl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kygmcive.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2hofjtrgk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2upkyeihc.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2rxfpfdjb.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2ssaqdpjj.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2gdgdmxhv.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2mkvnhxwy.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2fleaciwt.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2qeqjanyp.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2bjesugxv.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2mhapvqbz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2krjvlxuz.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2abbsdsaa.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2tfrreldy.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2jkdickai.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2zzljtmkj.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2gfrfihfd.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2esttmkab.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2ljirixdw.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2obvcivpx.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2dzgbybnd.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2xzyyzatd.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ivygfspa.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2kzyjgaih.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2xruwkwra.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2rzcpmlby.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2lgkzoybe.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2movizaky.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2dmvdjuor.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2fyaeidfg.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2qfwjtoda.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2btwpwzjq.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2cbgfwyhl.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2cvkhbioo.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2khagmyix.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2byxucpfo.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ofcijsxf.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fjcjwxom.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2ewhdlyxd.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2byhtdffs.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2debtzztj.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2klehpxjc.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2uhdpnpvi.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2tthwgyrd.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2yanfsngh.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2szydtpqg.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2mmbjzmqf.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2laxphwez.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2kqkjsftc.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2wsejtiey.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2pihhzzku.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2deocjlro.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2hwjwntdb.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2lukyxhnf.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2nnysqyql.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2fwpprixx.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2wdfzkjup.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2symxyadm.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2bztetnic.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2fyycbsdu.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2cfoevigf.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2jbijtsss.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2mzeijtnr.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2cwapubbb.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2lxautxnb.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2nuowmsox.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2hmzhbcph.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2doiisgwa.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2puehkocs.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2gbaqequy.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2ssofwiba.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2jhatlcuc.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2rwkxqbrz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2zvrnwfwx.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2ugeypzkn.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2ocuvadvd.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2nhjzdcqh.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2gbkyhbqz.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2uzhotewd.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2tqacsuva.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2icswaxpt.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2jthlxvnk.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2xyiyxhpb.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2hphlambe.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2tzlskxxp.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2abnixwwl.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2qinbweqi.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2qhuhktgd.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2ikvcjqcc.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2imywdyml.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2xbtyhkqv.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2tthwyjgi.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2vopxhxhe.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2rtvembwh.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2izbvldda.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2rmrahotg.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2oarwunhf.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2latlgeeu.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2llwnilyh.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2kvndxovm.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2kdrntzad.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ujxhkeny.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2nlukhpup.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2vmzfundl.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2vlscopcw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2zndufaxs.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2sdpungvi.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2mromgvaw.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2iilrsggt.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2kdafjptf.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2wjtbebft.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2btzqmpcn.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2jmqfrxhd.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2nkiwbrwd.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2mkcweffm.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2ibktwetr.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2yedorghq.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2wbtqgmss.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2pgvltzgz.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2dinklcgj.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2hyaubokb.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2dtjbcolt.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2nmozmpfl.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2ngifmaul.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2chwchygo.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2yvmyehtg.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ukmtniez.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2uvuoyevg.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2sqvytpml.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2kcqikntz.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2yyykekxe.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2mdwunpyi.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2uwpofggh.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2otnhhbkc.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2lqjzrbkq.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2dhevqikh.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2cbusnwsi.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2qkqccwvk.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2amugknal.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2rkebxrhg.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2lavnaeaf.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2bjsoxkjs.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2fxgklmrs.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2koarcmzk.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2mbtephkw.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2tbyzslnj.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2zwciacsb.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2jaiinbvg.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2zasmfsqc.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2ztjzkufh.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2yuamfjfk.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2zfyskjos.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2izcwlgef.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2boyvgsfe.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2jkvmuuty.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2zxpzmfmh.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2iokcfzgj.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2dhmowrtg.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2pqdiflyp.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2urskgsvq.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2yannxkdm.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2imuumbbu.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2jtqncqez.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2ymrcxcbf.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2oggfsfck.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2wgtxjadt.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2qcfafwwf.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2qttzfosx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gvxtyyij.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2hokbwbgf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tdyeufqi.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2poqueflw.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2ufpbrxty.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2nihdsbxy.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2jsxgmhio.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2agilqhkf.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2zxexxgpi.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2gbjsxlyq.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2jvdxzjob.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2gcfambmd.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2lprogkpv.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2bdumnvdt.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2nwotlvtn.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2krzznfun.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2qmmnbfng.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2gyjudfem.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2ovgtdgvv.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2pudnnlqp.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2rruwjoum.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2bwcgclwh.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2rluhdpws.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2djxffhyn.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2dacftpgv.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2nhnavfmf.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2cnpiredb.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2bofjokuy.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2ztwgystk.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2vswmvhwk.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2bbdrsbra.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2xorwfqod.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2gguujjzd.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2tsytakrc.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2nslpingk.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2qqpmbhjd.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2norsamko.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rhrjyzhx.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jnbzvanq.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2ohxfjuuc.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2fsryfymr.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2cttuqqkr.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2gohgamqe.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2odlxlfer.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2thedmxuk.html


<!-- 参考信息 -->