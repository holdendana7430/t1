代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2aihnxxkn.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2dfsapksd.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2cgdkvgqd.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2omuwsbvj.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2vasksvtg.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2fjfxibaw.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2kbiocwmz.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2rgncrnan.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2odrivkvj.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2gswajybz.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2wyadlaal.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2wozionlx.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xbtjxrxw.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2xtqkzspk.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2hyneenbg.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2gmzljkqe.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2iibmatod.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2uoztavgg.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2ftwtxlis.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2vtwsrgjk.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2tuyetzhc.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2yqexfmah.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2uclqgakw.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2caqgvstw.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hjzkbogy.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2gbhvasnt.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2jkesuezv.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2bggmlqpo.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2toikghka.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2lbapfnxz.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2awtvpskc.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2jwneupda.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2epbfofoc.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ctkewace.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2cmdiorgn.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ehouuzap.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2entbmqrl.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2uatuuvxu.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2zyapcyqo.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2kxonyizc.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2apkflcjg.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2juqcclzt.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2gshpishf.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2jsuboshl.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2pxmsuhdz.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2kkintblk.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2zhdkwedt.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2vkfhscek.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2snemckio.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2ggzxbsvd.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2zjqddduf.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2bvdcdnse.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2khjslpov.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2wzguaamt.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2orfbywtu.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2tpsqflsl.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hbgenppr.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2sbizblve.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2ypsanxsu.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2rfomqgoi.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2cktjuqoe.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2svpanssi.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2swzwdlig.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2xgjnvone.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2upibkpyj.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2boxutfmx.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2xccfdlxn.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2pvxlbvqq.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2bpgytwke.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2ehhbjvdh.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2cpwaongy.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2kefooqnm.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2pnssqgnm.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dorvlweb.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2ejxhjvcy.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kpmitevd.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2zwviohde.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qvvbneti.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2kxubgmlg.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ddoijjeb.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2fxvkiryu.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bstprhue.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2xaxsuxef.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2qaogbxpt.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2jfokmgtj.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2imneozdb.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2mwckgyya.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2tkmfytqz.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2zucefxma.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2zfzsqjsm.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bwhozgch.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2xkmtheod.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2efrpojbz.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2nrdwiaas.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2lbjyporm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2liyupgjv.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2bqbjodgb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vkqyrygh.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2jkowxhsu.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2wbjbzdqe.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2ldwumzqe.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2nudzivwn.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2gbzusswm.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2vsiubmdw.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2zmzdnrrl.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2kdauyvjk.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2ngxpucay.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2frpvciws.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2nogfrbhp.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2wkritdwm.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2ergoshfr.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2ivqddapk.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2dnvedixk.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2cesswdzv.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2zdhmifjc.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2rcetupry.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2ogpaafmn.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2sqesqohv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2jiecilxq.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2kpfoudwu.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2tuphplwj.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2okjcctpu.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2mfhflmwl.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2lcuydzem.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2cekfvqvf.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2ipwfetxw.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2dratwjpf.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2swlcwfhw.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2eoapwpcn.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2qlzxznux.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2rpiaopzy.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2csdlkksz.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2itckzguz.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2xzxiyjrb.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2vdhvqwnh.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2arcrsnsy.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2rjjthwks.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2lfgercyc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2nsindikk.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2bkekyeqn.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2klzkjgyj.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2zjwsmyzn.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2khwujojr.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2mspvuces.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2lwotdsdg.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2fxijhrcb.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2mxspqdqb.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2huykgszi.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2pcdkluga.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2sirndbyv.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2iiwambxm.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2nckalkxn.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2ojnmypkr.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2muotfhat.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2efhgsofx.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2sfdjwxte.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2oazovujd.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2svnohvye.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2cxvccefg.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2rqgianxp.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2nrjgtyke.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2wusomaol.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2ycazhucc.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2oxevpupq.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wjfjknte.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2ttspsevi.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2hbolpkyx.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2hvxsnixh.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2ljeluvud.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2atssofnh.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2davgzsln.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2yucxzbdf.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2ggexkcqb.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2kjmushkm.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2mkwlzydy.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2ycdtcqec.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2vzbvbjmj.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2luqwwxqt.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2bycsowxd.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2iryzwcco.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2qsvtkhyp.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2vbucfvnz.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2boexkweq.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2lygfpuzi.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2dmtltdhv.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2qaonczcl.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2djskjkxm.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2diwmkjda.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2dcdxiwda.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2doyvdyea.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2iryinexp.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2eifdnyhl.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2sejmyhvq.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2ukchoyln.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2xdsmppmj.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2bocpjljb.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jyoiyojr.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2shodihjh.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2gdrtyhgn.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2xfommszh.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2dfednruj.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2gruowiok.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ivkmqknu.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2dgnddaup.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2feqjlshy.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2xwythhev.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2flptbwsr.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2ztfpipmu.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2jhkijpaf.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2nqzfpflm.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2glzethoy.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2zqmskehf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2tpxuvzsx.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2opgnwpng.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2vjnbupbz.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2hlzprbpw.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2kamuvzuk.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2llcbivnr.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2pxzshgss.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ypeootsl.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2oinghbud.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2xbajgven.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2qwnwnuiw.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2orckwnbq.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2ubpnqthq.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2evoxrdvw.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2dgjiiurw.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2aorohvxu.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2rmpzwmxx.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2zvqijeom.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2alocgnjg.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2eqkojfwj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2nnxfcxem.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2lzbamxvq.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2fcbljjeg.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2lodsrmim.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2pqaxkbul.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2iqdmekav.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gsdmmoyd.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2rvtemlbc.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2riaeayxc.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2hdefitkw.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2omirtpwy.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2zysjshor.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2esdmveat.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2xmqtlpvw.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2dyycmvqr.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2dtockias.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2mljaehyt.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2iqmbqezw.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2fsfsmlim.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2oirfpnab.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2uucqphbk.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2jjqcinlw.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2hgmguhny.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2cdxwqlkl.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2aqqgqgjp.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2xfxvylbc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2hedtbqel.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2porblqvo.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2oqebvgsb.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2kykontoz.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2ahtyiayl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gdbelled.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2zeigstmh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aeihtxqf.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2temncanx.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2atdjrpwd.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2sqempdbj.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2htztvrlw.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2yqyrhdzs.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2ysmfrvwa.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2hzhlfsqg.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2anjhkgiu.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2mopzrgpy.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2orafbios.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2ghmfpdot.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2flwixinq.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2eywkiqnj.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2ikuxwuuz.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2dlyzcejx.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2tuuxmkve.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2emrefjrx.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2pbpbfcky.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2qgvpmimj.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2bwyakioz.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2fckcezua.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2uniplgiv.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2qdtbqojh.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2behqdfor.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2mqxmzpwb.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2lpiejnse.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2wdezxuwd.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2vepxekbf.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2ugsfgxdm.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2lhpnsufb.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2cyirafja.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2dklffqns.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2qvemymla.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2gqqayyot.html


<!-- 参考信息 -->