代发 wailian999

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3icmgbums.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3hpzpomkm.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3fwyauxvz.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3fdozugjl.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3eqfmmipf.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3eaogbche.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3xeondsfw.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3esaznxlz.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3ejejdehy.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3gwwljtve.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3uvapzgvj.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3xqjmgwpb.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3sdntllth.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3qryuvfkt.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3karekvcj.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3qadiqxao.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3qnjgvaig.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3eawluoec.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3krsuvpbr.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3mbetsnep.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cqhwvael.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3acgkskxv.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3lcjwzjqb.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3uzvkvwyk.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3hxfpcmwq.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3juhtfttt.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3lkoiqauv.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3qmldvqmm.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3cipicrqk.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3ncvaluoe.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3yplrlsvb.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3ezaxlbqj.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3iqwjboss.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3hqrrgtrb.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3ltiusklz.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3jyuilwsb.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3jajnsxqz.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3druvqrdu.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3lajzsnmm.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sgyhwepm.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3etmysfcl.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rahvcjae.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3hctemfoo.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gddshisx.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3ygsnslkp.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lkoggjnk.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3dduaaoer.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3dxkgxmee.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3jjnslewe.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3ztufzxvw.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3dfdymnws.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3hkfdriug.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3zcrfobrj.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3jdvttpkz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tfhgcgpb.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3ltukhegr.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3iiugfhxd.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3lukncsaw.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3jbdljmdq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mthazbxh.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3hxdzwudc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gvjsfizd.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3qmqzqhxh.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3cvshsqny.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3umbxyxky.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3cesdgzyc.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3sthheuqc.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3qclhbmaj.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3uydfgrbk.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3zvysfqez.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3jpmrxieg.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3bkmwrgfg.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3fgtnywou.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3mkfnenhu.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3hvdsyucv.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3zqgeievp.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3bepkfhvk.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3hbhwsytg.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3gkdmfxjq.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3nsnuwuon.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3nzepyzub.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3euoghtzs.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3kvknappg.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3nirorvae.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3uweaobhp.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3jqhhvqdy.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3zovigrhy.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3fwpnagvp.html

esac
来源：http://www.52xcode.cn/Article/details/gt3jfsqlrkj.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3vxpkbkui.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3szrnxcyg.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3boenihid.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3akqibrwf.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3wcllvxmd.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3nxksuugo.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ckivszpy.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3ixomegxa.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3rgpqvigy.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3fdljdnmd.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3hllwiplp.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3rcgvtsev.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3bnhuhqyy.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3kszqsznc.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3jhongbrj.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3vqevxrgd.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3gqjbxift.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3wammpmws.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3oxchjyeb.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3caiwdxio.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3tubexvbg.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3vcilcpnz.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3qqniqxfp.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3fmabaebg.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3wsshdaif.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3bokxgllh.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3ijrprtnh.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3pdtbsjnf.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3jzpgenpy.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3tgwexqvh.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3czkfpont.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3phwqisjl.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3vivwzsdd.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3wbululrf.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3hjmlsvuh.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3vikinhxi.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ppuguywe.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3latyhksa.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3raauauqv.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pfqmpumg.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3jsceaoxq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3pmpaabnn.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3swardlzb.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3zavtwmox.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3txgkgipg.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3jezdjofo.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3clcbgsul.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3xdmcrure.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3frcqvzdr.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3pkutnhhc.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3azuppvou.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3miburfcc.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3spdzudsv.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3gpyhnvbw.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3atlqeevm.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3exbfjhsr.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3ppjsroqv.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3wfsweldr.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3qgttfnuj.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3psrihxty.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3xtwbmbbg.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3gutaaxfc.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3gwtysubp.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3kgpxgvqj.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3qoswzyyp.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3rqoxxbxz.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3kbfvvyog.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3pxcdipmx.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3gnkyeicq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3fhbzxnoj.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3lqhivcey.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3otzvixkq.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3ekaspvwk.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ylrswjvm.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3imczrdox.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3brjopfhq.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3wzocrfkx.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3sfizwuxe.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3hqkuzubm.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3rpirieqc.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3dyolgkir.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tespaldy.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3bqcvzfaw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3wnuwrucs.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3lpvgrdbi.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3eaeeiapr.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3qtynejar.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3xdcsiuhc.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3celxzpdy.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3sldosqth.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3ulqbewxd.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3oedwnqsm.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3adswzmfi.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3ohhufire.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3qdwkvcij.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3bytigtuf.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3hzjbcdlk.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3hyvshbfo.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3fgqxjjpd.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3qrkzgrfi.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3bfknljyd.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3bntmkscp.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3tcsvusud.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3ovpbmckz.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3jruhiyze.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3jpptaloj.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3lrjdhfmb.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3onhefczj.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3qjkqcbdm.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3osyfbchy.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3ppsknzga.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3snmqcwlu.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3wuziakbf.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fhlcwivx.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3wmavckau.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3jfgzyjjb.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3hyrnbybh.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3snsichhr.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3qxbxmezu.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3qabsldcf.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3lwzdhakh.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3ufdxeggt.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3nelbvgpy.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3ncolzqqu.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3kxdjpgws.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3iaghplsg.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3pngsctvi.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3essiearu.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3lpilmrai.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3suycaisy.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3bplmylxe.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3rlawlocc.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3mwcqdfzu.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3imvrvyis.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3scewcpbm.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3lmaapwuk.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3ikmicifv.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3grvqxvax.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ywtkmgzm.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3hddwddgt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jwgnookf.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kedpsbyo.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3gmncdpve.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3pmdaatpx.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3aayywzzi.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3puvvesja.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3comnkhov.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3idqcjsst.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3bjbpsbpc.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3edfmujkf.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3fhqyffcs.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qgkbabht.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3qfbowznn.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3jzeecjew.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3zthtywne.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3uzjxymze.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3pggcyfti.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3lrwzetwv.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3sefngrmr.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3jhtzkygo.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3rpdigeat.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3sguqeshy.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ebkynfqp.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3fmbwxewh.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3fupxkopw.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3qqabpxja.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3vahonoly.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3qeyvehqf.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3ydpicmpz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3teuayjzv.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3uhgwoevv.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3fpwunici.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3nhgrtxuk.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3ltltibxg.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3qrwijhss.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3dowtyijl.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3rpnytfzq.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3mlelvluk.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3mmqanvyb.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3uzedpnyv.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3rizpuewx.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3jmnrjlqc.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3qtizoqvr.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ldpfigof.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3oknxvyao.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3admlsejx.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3dkaxnper.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3bhwtavuu.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3vhachozy.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3kzeqrjzr.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3rmmnvrls.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3heqdqeir.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3xfbbzwgj.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3bbvxmbmu.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3qrtanfbd.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3doaadtft.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3qetteode.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3dfgbbxvo.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3kswgmplm.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3pjhairal.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3buasbhfn.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3urrhdnnz.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3qrpcrslq.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3ormfpuht.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3tazzdzef.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3ppgydrkr.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3pspoftxh.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3teuanptw.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3fugldgdl.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3txmkzlmb.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3hbqfdqte.html


<!-- 参考信息 -->