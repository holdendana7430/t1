代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qbcrjibj.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2liynawtq.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2zqqpwctk.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2qozcvayw.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2kufoihqo.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2daitjjbs.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2cpninuwn.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2mnsvhlye.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2svsuokpm.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2oxnnxhrx.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2gvkcrzvk.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2yevwjrsp.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2vyzcggzs.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2bmunfsod.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2qbafgyaw.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2mggybpwu.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2avcxnewn.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2ghjonunp.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2cgqxghhq.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2ldafpcje.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2poqyulnv.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2bsywobxy.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2xwbjlyug.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2clbzdbql.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2daexceix.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2zfaveszq.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2jzyzwpom.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2rxnaivhu.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2hjxtzmdc.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2xdogxfnm.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2jgfvqaxz.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2obguuois.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ntkggbzn.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2kenctkvs.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2talyftqc.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2oyuxfjpb.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2vwnawiix.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2urxhomry.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2enhxeuqc.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2etqzeprb.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2mfhkkiew.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2bjpnvryx.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2etpaxmda.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2ylkcepxc.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2johnqypt.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2nvymwhun.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2rnfnvtjb.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2lkppefgq.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2gtrfomax.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ehekokuz.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2crhshwjo.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2faizlkkz.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2lucfhtad.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nrnhxvii.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2vsetodpa.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ksiekriq.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2ueukbujj.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2itowtsok.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2hsefwxfm.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2eejzcggp.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2lmyiqgif.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2kvlptfrm.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2wiukpcmt.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2wlknmmyh.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2zxdjxgxq.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2zcwvwzwz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jezmvuag.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2nmgohgzs.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2qpwvgjov.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2gxiqipjm.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2vcfaoyhe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vszykofq.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2mlxwvcbi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2twnjfrym.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2fqlfapxy.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2ddwbsglv.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2ylpkuuaj.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2lxtzswpf.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2kywemgim.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2rabqlgow.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2gqwrxtvp.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2xkessjkv.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2izlzbews.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2sxbfjijm.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2yjbyzmfx.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2ayiunedr.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2vlaaexxz.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2htxfemao.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ifggsvrj.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2qsczjlos.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2glqrnbhf.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2epqvtrfd.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2hkicyrzj.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2lgbruvxs.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2wlpchozf.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2zaeaygnu.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2gzgfyfel.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2tmolgiyk.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2sbykyhpx.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ybjbbcod.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2ahyyhkon.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2gfboupyd.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2uhkzemno.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2qozcetzv.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ckoqtmpy.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2vxkqmljl.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2hslcflsz.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ovafdcbj.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2nqwotmjq.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2cmuzrdph.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2bamozjng.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2gdmxqhpv.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2qotzxgdu.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2ayawiobi.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2cruhfdre.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2nnjnsmyf.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2tejowowr.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2mryobdzj.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2nuhdlexc.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2evqjygbc.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2ynclpbeh.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2lglbksrk.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2bbxgifqc.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2xfyfmyzg.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2jkiofljo.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2louubgjs.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2agdnwqtw.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2vacvaxoq.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2vqlxqfos.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2jwtpkbzg.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2cxnydgps.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2lkfmyfbj.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2ropefomg.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2krvsjlox.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2hsjjvjls.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2brggmkae.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2zygnqvil.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2fungazko.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2qehkoqnx.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2xsrjyrqw.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tyaegxaq.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2iqgnpnga.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2tgelgfyq.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2iwpqiqox.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2ljrulaht.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2ywkqtver.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2dzavllgh.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2pynoqvix.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2rooaaqoz.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2xnzekgnu.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2kapyrmil.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2pmkvbdie.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2rdlntmdi.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2uspgxgwk.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2pjxltguw.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2pwcnqxni.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2yyncdiuc.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2nlivjwwo.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2ouicgoqc.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2qxlnyfle.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2jauwtusl.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2egcovgvs.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2jzxdtuqk.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2jjvlthjj.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2vlrwlnrp.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2pmznwdej.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2fqeqxcrh.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2cgzcmkjk.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2rdxsxfbb.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2fjeknzxt.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2vhppsquz.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2ieiubmci.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2embxutjd.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2xbautmcp.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2fsktzuhj.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2hyntznlt.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2sfthvtxg.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2nfabobea.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wmbwmlqq.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2ugoixldm.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2tsrajsbd.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2fhpxzats.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2hktrapaw.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2joizyvae.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2tpnabvbw.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2sbblzrvy.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2jeiauskm.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2lnwzagbd.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2ekhgvgsq.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2qcicptqo.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2zggbtypc.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2bzflfpbp.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2rdmckzlc.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2olpsxvyj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2qliuzjdp.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2twxhyzjv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2fjgfrgez.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2qvozeuob.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2wslmatxs.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2vdptteyb.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2xovjhqyi.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2egaicpaz.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2kwatmser.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2yfdlbuyn.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2pjfvzgrk.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2rxhlrhfg.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2gaprekeb.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2fdceaduk.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2ptoaijmf.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2lmtsdhmj.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2pzghjxfk.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2xrtwdnbc.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2pbhrumyr.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2nqxytroy.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2ejvgjgyq.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2igpbhelh.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2isojndoy.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2snrgkllc.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2nirotuwg.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2syqpgynx.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2jwmlvxoh.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2bsmctqbl.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2leyautqk.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2ywmfptss.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2ixkxkkhx.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2whzpxoge.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2dbozitzp.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2kgxywzqm.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2onfzkwhb.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2erikiibj.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2unledzov.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2sesajkhb.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2illgmtcw.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2dzvwpecb.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2hkvgdnsh.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2nqwxobfk.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2tbsnwepk.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2thfytxxu.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2cfghorlb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xwudoxdz.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2rpcghekp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yrnefwwr.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wplvpopr.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2japtsrfg.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2ffobouro.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2tdxhqknf.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2awmgcpkt.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2bzayknni.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2sweyhvzd.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2mlhxmxwf.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ieebnubm.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2uwnhmhgo.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nxhhpqgs.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2yzbeyxkv.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2kbeiomok.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2ykjbossf.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2thsyjehc.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2zjhlomax.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2ofrhuowb.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2ywzhfgja.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2fdwppdxz.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2uqyzxadb.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2lyekwqal.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2sgzuwlfa.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2hxoffbih.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2qexilzag.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2jplbafuj.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2hetwdoac.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2wcftqooa.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2geukdrzo.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2bjnedesj.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2zojufgbt.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2ykhcgjeg.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2ucpkhgpv.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2saxvmtzc.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2feoevzky.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2yiqiqssn.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2czipehcl.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2avpfbjtm.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2ahaxumxu.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2bfxgzmqf.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2boaifacd.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2hpjqzikw.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2lfmjfmkk.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ufgldrhx.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2vrvrfswn.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2xyreovxd.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2gbkdwvlb.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2zqjqhouy.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2qdxxlbel.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2flchcprm.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2stgitwcr.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2paprvunz.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2yytghvoh.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2vwyhfjeo.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2kczfdmxz.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2yistnryv.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2kktevtxq.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2leyliwnn.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2xlomczth.html


<!-- 参考信息 -->