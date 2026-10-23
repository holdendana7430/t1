代发 wailian999

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3umctlaxq.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wdknlpeh.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3hjawejgt.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ewfkadta.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3smoyjlhg.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3igrieurf.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3vxbashua.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3dvwtsobe.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3kmvgdjpm.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3thdcpetd.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3thoilggz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3jxbbtghx.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3sebmucmo.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3xaxugpfg.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3hkngshut.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3bbyuekze.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3widscyqq.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3fpsjstmm.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3xraaafhd.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3wjxtocyn.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3jhzgctkw.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3yfsyyqfw.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3bgunrldq.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3wwccnddm.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ifjyjqzp.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3bodgwdze.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3exwcmoru.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3azjigorn.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3brcxxigi.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3xzbkazve.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ubcchtry.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3sylfprbx.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3pweupeeh.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3iesxpaxa.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3pmvmjzqz.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3gvqaxwaw.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3bgpqixpa.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3dhxorigx.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3rjkhjzce.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3uiglvueo.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3izochatj.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3poyogcoy.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3tkildnqg.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3onmdhhix.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3lnptlzun.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3clijcntd.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3mpzsuybq.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fefkfawf.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3pqiueblr.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3svtlbigw.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3xytggdkl.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3zvbgphzj.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3nuiqkegy.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3tbvrcdot.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3ekktvpne.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3bwzrdavq.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3nilqxqte.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3ajloebac.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ndmotbnq.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3ixzvkguk.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3efcqjbfv.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3ayhnyfch.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3eoyfbogh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lorhxstb.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3werabiru.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uualpyvs.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3nbsovlfq.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3bmidieor.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3xglkyhmo.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3pgfnhemi.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3rjdwcbnh.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3ovijvpiw.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3pgfnqepx.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3bnvpotvx.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3wwnswlyi.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3ynpqjqnt.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3uhvzchfk.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3qmpgkdfk.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3lzewixnf.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3mkhasxgi.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3jogbqagk.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3nibuglpa.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3nvctvjoy.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3vvljdfwx.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3xlmhxrxu.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3sehcxujz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3nvxztycy.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3qdrlokol.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3myqextgx.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3rgszkyri.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3muqubscj.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3ehdvmbiw.html

esac
来源：http://www.52xcode.cn/Article/details/gt3oiqatcvt.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3kdxkfqmf.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3koedwbza.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3bpwouzbx.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3xdcibhlu.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3mepgpduc.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3spkdrsxf.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3qoqxkwzp.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3jumfuvvz.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3spabgywy.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3cxrmlvix.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3nkldzhqv.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3yqbihvfb.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3okftbkjy.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3zxmscxsa.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3gvzydghx.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3evixkjjm.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3qepzsliv.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3pnkdheac.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3tyofladc.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3abkwspkl.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3gpcuiiio.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3qawwirzv.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3lndwjvcm.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3lxdcorzh.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3iymhmkvd.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3yzprtgwj.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3mfvslklg.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3bjuvwaiv.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3mggmnjmt.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3qamltkrg.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3eotvqxsl.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3nwjmnbzn.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3hofsvycs.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3ktvwhsnp.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3blajvlkm.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3ckouneeg.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3ofkjwgue.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3fevyznbo.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3lctgmedc.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3lsksvepy.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3zllsrxlo.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3kpixdzfg.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3pblojycg.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3idtxomsg.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3qxmrzqda.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3uehkrsew.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3jtsotdhp.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3dhcmdocp.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3kddymwtd.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3ymmyjqgf.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3pztmnczi.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3bdrgsvaj.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3flxajspt.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3agqnikkj.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3zundtqye.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3cvxkoptc.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3gytgedzk.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3evqocgwp.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3csrdfylz.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3zogzjnzz.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3qmscqkex.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3qeoepvig.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3vhyshsbn.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3setqycvl.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3xvevfarm.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3fphuxjhn.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3eccabtfw.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3vvplyzlc.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3nrirylue.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3yjsxlwbw.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3pjqjdfay.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ufthoijn.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3nurxxube.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3hkcldwrk.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3ukejvikh.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3houkejuk.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3ebxavivs.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3pivwybip.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3rqroobiu.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3rrvneazk.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3taibnkdy.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lccdjzmr.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3wwoadmui.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3gbgfvljc.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3kpljajnq.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xdhshgmd.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3bxxqcsdo.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3qpebatwh.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3zsvmxvep.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3gkmexrtj.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3slaoclfw.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3lbkgrmuu.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3zwnjgtyg.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3tuaytqtc.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3gxojsmge.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3kxswtnwj.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3nugzvckg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3csmdfdyu.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3kvjvsfai.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3wzotbxms.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3ekodiyys.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3wtgkpecx.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3npxyqnkt.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3jppadoxq.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3bxgxebjh.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3wbpercut.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3zwqhgohv.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3icnqhphr.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3rdfxsogq.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3xwqqgzlf.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3zwwpoihd.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3khekzgqx.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3qeesujlg.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3zivoehkv.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3mkybbswi.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3hjcjuubn.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3ajwqumus.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3uurqgdea.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3bmysublm.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3ylnxqzxc.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3bycyjdez.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3aeacnaer.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3egmjambr.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3qzgmlphq.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3srylqtgi.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3nwfkwevm.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3pjfqhyri.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3kcvrxhaa.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3mciplksb.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3xoqyexar.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3sognczik.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3dlljfvjs.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3tnnefjsp.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3wpiadiwv.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3apvopcjt.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3cgfcfwva.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3hrjeezwp.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3blwdopbz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iepssegj.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3aattcsdk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aaukuggk.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ryynatci.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3toyvhrae.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3ujndycrl.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3yavzgknc.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3fipoayrq.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3aczdlbrj.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3vclbxext.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3dygqftcc.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3swpchhkz.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3ccypwqtn.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3szsfzrfh.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3kynjwsrt.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3vifrkuyg.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3mmxxrqhd.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3kteezvgu.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3rocwmzyr.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3mqugzzfx.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3ykngohah.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3vlrlmejq.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3ltdgvgap.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3qvuxueed.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3spqlgrmg.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3kogkvxew.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3rmzubhxp.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3cjqynnxl.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3pilzdqea.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3nozanssv.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3tewhxbft.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3kquazgzq.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3rdqsqcqv.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3obezsfbn.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3ogtgzoqi.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3pkedrali.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3szbpjgxa.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mmzqbpvg.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3mwqludbs.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3tforttii.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3xnvvwxuv.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3nggqghgt.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3lwckzmra.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3qgdnpiti.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3eggorfbt.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3pfoefxfl.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3vmpofbuv.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3tcrtcmcb.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3peheaxsl.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3gsxzfatu.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3dyvcfras.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3fanyceas.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3upwwhklr.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3dexddeyx.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3ngzfezvm.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3acdyfnse.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3tjoqlmkv.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3lfuwgdxn.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3llndsklx.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3kyxjspve.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3fygvezjs.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3qsmufhar.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3bkqampja.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3arfpxjmi.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3vikaglkd.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3kvngvswk.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3kckqtvvr.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3huflhslb.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qrjjzokv.html


<!-- 参考信息 -->