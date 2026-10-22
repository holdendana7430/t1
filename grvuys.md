代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ivxzwvju.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2cenhlrni.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2xlghtyhp.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2lhhybnki.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2cnlpnmzf.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2pxxdzewd.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2oqvnxbqm.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2mttwcqgn.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2dsugchsf.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2bvlohhuz.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2gtbnxraq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2wlvrucgo.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2kewspsik.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2hpnnhhdq.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2robcgvtt.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2lqqvcfzg.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2oacdqbvy.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2cqgfocfi.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2viusibzh.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2abckydmp.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2klkrqvzv.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2qkjzrjro.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2tefvjvvw.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2jbscxazc.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2yhzxsasl.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2msfbnozs.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2xoqxiqsg.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2qpuyemcz.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2cpvdhqga.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2rvzttrec.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2jwbklggm.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2sefampxj.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qkudxjnu.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2djcagtku.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2kqjfvetz.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2sbhusxhj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2pvkxwgce.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2lpwohhck.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2hesdvaxx.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2zqjokjus.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2cvzojfer.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2gejjmira.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2owxxfysd.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2ytqykcbz.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2ttkvtvaw.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2sxeijsui.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2amhtjeto.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2hbcwnjix.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2tvduklqb.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2eysdwfcj.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2mnziwlqc.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zjbpwsva.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2nolhcgpj.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xgquebta.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2hlqerwep.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fwwmdvrx.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2zndwgagt.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wkpkgfze.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2zrrmbcte.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2wrcsjtyk.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2tidzrqlg.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2kdtwdpoj.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2guccyjxd.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2scdcnwne.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2nhtyhxxp.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2zgnpcpkf.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zjkjidln.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2wugspzug.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2ayegzqvw.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2bwzccuna.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2ivyyazmz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2olbjmjww.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2mjhqiump.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2puuxzgur.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2ytekpewy.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2msqqlkao.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2tufdtoem.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2qrzvwgyy.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2gffuvanp.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2pbipgxhx.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2zxiacmsa.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2qevvptih.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2diireewn.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2qhaexlqr.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2sxwqyeur.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2aukvdrwq.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2avgyntqt.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2cqmpthmp.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2fkjdtwlr.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2tdbmsisq.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2dihpjhgu.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2yrigncxw.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2xhcabeqi.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2nqhuvlje.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2kfezqzxc.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2swnlklua.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2yxlndcny.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2natqcywb.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2crkzlvxl.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2gwahjrbx.html

esac
来源：http://www.52xcode.cn/Article/details/gt2oberxrfo.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2wswmatak.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ijneojbw.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2yaxvqtjz.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2piwhdsxn.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2kvveverg.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2dshemwis.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2lllfqzrg.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2cqhlokkq.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2cpbwngoe.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2ymbwnsdk.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2ocglblym.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2qqydyflg.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2kvdcjtbs.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2jndjpqim.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2bdgianvi.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2rpvnoyau.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2lsaypfew.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2tzyexbyx.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2qfapoedj.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2mdkknbvf.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2bzhpnoeo.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2ypnvivcz.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2evqkkwjb.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2uajdbckt.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2tntfhfzi.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2efgkhzjq.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2bmsxavwk.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2sepoxxnf.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2osxgtvky.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2utycudht.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2jdydjgct.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2xvnhlpnj.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2jpvebiqo.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2ljjagtjf.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2tisglxfy.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2ibvpdlsi.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2jvffvozn.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2kulishql.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2uduvhihy.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2uvqdqfsh.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2vneeysmd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2ukerwelt.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2bqijggqr.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2dtbnkdze.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2wvvehigl.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2iffzpkri.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2jueicgvu.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2zfxtkwtx.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2ijyvbsfx.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2grgpjuez.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2eptmvxke.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2qzkxhubc.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2icaijpdk.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2altvouos.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2rhlvrjfa.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2vxvipwxf.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2flimwhwf.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2jnuehmkw.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2zhylkysw.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2frveozfu.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2rjpaenhw.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gxcmnkwn.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2jflgenbt.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2iskmfrer.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2gvbmhozp.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2zlbfiiqb.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2lubdasnj.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2jewcrigz.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2aqbnyvbb.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2ijyvsdlk.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2jcyygrtu.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2vbpjlgev.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2bkcwdidb.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xfxypvjf.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2cgoalvwn.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2imrbctql.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2qfboqvpz.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mocnjzva.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2skvvcbhv.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2stkidofw.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2jyapuucp.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2zhjkyklp.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2qwtbbgzw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2uyskqhmo.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2gcnesffr.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2fxknedzc.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2uglmrqyg.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2hzozlcds.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2rtrxnepr.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2xeudirur.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2ygelgjfr.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2pfaprnmi.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2bhzpmtpw.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2muwlnrbj.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2nbdtzure.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2eqmrddpk.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2snzxepkg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2grcoxxmc.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2rpjmbfqh.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2welvbmtx.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2kmhckpkw.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2bohewgci.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2qodcpjfq.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2yerljyse.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2iavblpxm.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2enpstgfy.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2mjbmefta.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2nphqlglv.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2mubthnvi.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2dnosclcy.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2oeqqgjwm.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2mjmjhxno.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2tymcsukh.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mhackgsu.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2bkqmtljz.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2zpcpdixe.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2hhjgewwa.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2tyjgplij.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2jbuqiati.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2vtnettof.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2zjxdajot.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2tkmoyban.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2ugqzaapz.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2yqttejei.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2wbfwxytk.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2hbssxufq.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2hrrxmzsh.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2zinywftw.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2puxhxenj.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2jtxtarut.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2nqyfgjtn.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2dfnymseu.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2ntiwwgap.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2ptrdzksi.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2quimheog.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2mjvywkmi.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2fcubsdxy.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2jktoaeaf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nqybarmb.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2lxaatjyo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2stncpwbj.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zvkpcnyz.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2bsdokikw.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2mgptudsx.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2zcolyjfy.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2ptvqmafp.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2oqstqlcr.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2ryxuhvrs.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2enedjesv.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2phgdbvzp.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2wsaqpstt.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2fqmlwxlj.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2notjparz.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2lsjvifst.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2rjowlojf.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2rruszrmb.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2qnocnqyz.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2gkozegrx.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2rdznehxm.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2ltbvaalp.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2wvrciros.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2khrppwwe.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2dodaoxti.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2kemaoaer.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2efuealjq.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2ndzysckl.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2geyafzrm.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2jrgcdlwr.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2qubugnjg.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2rxuecnci.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2jmnaegyk.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2rfxpswyn.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2cobryepe.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2tqctimfk.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2bpbvbcjh.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2bijtplxq.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2yazywodq.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2txjmkmhj.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2jsfluwqv.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2xyfnmzol.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2xgmasufd.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2scmsryfu.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2lhuurgtr.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2nphkhikd.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2fpifsfeo.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2ypafkeec.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2zfhvamhy.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2iqvhjbcr.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2uldkcazj.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2xlvjrvib.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2hwsoirno.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2zafpknff.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2gojvtuyh.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2dckaiwfn.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2avynotse.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2zuszxekn.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2sxheeiju.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2leswdqhl.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2rwsqqzbn.html


<!-- 参考信息 -->