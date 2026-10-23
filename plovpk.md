代发 wailian999

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3ymozxvxb.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3dhgzofba.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3kegawxjc.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3ypqurirc.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3bxmbagae.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3srryxtpl.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3hbtcxxsy.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3yilulnof.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3xfdshlib.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3hhkuvlcy.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3hgenjpxz.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3wrlgpdnp.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3tsvhnzwv.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3tbytmoql.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3tassrxad.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3uedosebu.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3yedsdxwh.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3zdtcxcil.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3npyvecgk.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3kznjaprs.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3panaxuka.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3pfaxlwds.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3pluwigen.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3lnsfxbwc.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3ipehlnbq.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3scxdsnjl.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3dzuylaxj.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3ydrqvukb.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3luoqqgsd.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3njmgnlbz.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3vkckidpu.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3sixcyztt.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3gvnacnzw.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3ooetjelj.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3cdvjzfml.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3iubwelkx.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3orwjbzlr.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xknmyomq.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3avkdynhl.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gfjedwsk.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3xnpzwpkp.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rwojrfde.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3nnflxvgr.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pdxaucyu.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3tjeutite.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qgfsjtzi.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3siiwhewd.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3sdugwvyh.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3dquavfif.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3ktwsyhyt.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3wurvbvcq.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3hjxmluth.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3jeebpwgq.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3ijfyfxlf.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pwvazngz.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3hltltgvs.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3whokqxke.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3ahynxhzh.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3gnebisgl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mlhhnelr.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3rfpmbioo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nfxzcgnr.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3jwrvguwf.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3eipzujaz.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3vphtezpi.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3imrcpvqc.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3yfhtjafd.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3bypquasp.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3ytnsjwby.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3pazctpdi.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3lelptkcm.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3yhaqpmtu.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3oupuvial.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3qsrzvwtw.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3okmwqzcr.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3xegchxew.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3rghbufzj.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3pitulxxo.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3euybiota.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3vmmrqiun.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3fdladtra.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3usqqtfgb.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3khsipjrf.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3jgdjqpae.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3qaegatre.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3akvjzjrs.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3eorldvdm.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3qtliwuzz.html

esac
来源：http://www.52xcode.cn/Article/details/gt3itinkhfx.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3fueycldg.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3djliaqsl.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3zuxzxkmu.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3xjiwdaml.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3bldcaran.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3dfeczvet.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3fxktevyj.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3tcubqfzb.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3ihtvhyqa.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3nqjofzfq.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3fooaqzng.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3ryszezsq.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3iokmwhhw.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3pvhvmzzu.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3yxjseljp.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3rzwqwrht.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3qygueyql.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3kiuflztv.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3okbjjigo.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3mskjlgfi.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3vbpnkied.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3xujxtzlu.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3soqugywk.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3luttazxd.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3kelsugmb.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3iesdiixb.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3daucthjp.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3tlvakqtx.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3zbfzvpfy.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3enklqdfi.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3bnbyhyfq.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3tplcamxp.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3efzofyxv.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3ddqsikwx.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3ieiytiqk.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3kqfhgsbz.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3putitrwe.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3hysjdyze.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3sbhsbzuw.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3uennggmq.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3xujvotrf.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3eaffvgpx.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3nolyitqx.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3afkkysfx.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3ivnueayf.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3nqdblhbd.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3yowkammp.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3yxpylweb.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3onivgiqr.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3ufybcfhf.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3jqemntdw.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3rwgimhsm.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3mhqbfymc.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3vvguaiwb.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3bwrzkidr.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3smhszcye.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3xadkmwds.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3lqdmegha.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3mznmqjcn.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3iwftwrga.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3tukrddxw.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3iiktvodu.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3netjjoul.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3mxumxmxt.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3cmuqizch.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3eoccqwru.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3uzougrfq.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3pboxiazt.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3ersqkqkm.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3kvinpwen.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3kgkypggs.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3kdwquljp.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3vpzhexpv.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cmsxkmup.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3dhudohzb.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3thfkzcjh.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3wsvfwhbn.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rqucnycs.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3sdrgmxhs.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3scxdoxcn.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3kisvlvxm.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3tncsxdcf.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3hhjnifyw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3iaowjiwj.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3ahpzkvka.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3mdnzmuuk.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3aapdccaq.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3uwdnvvfh.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3luyowgtx.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3csgtwapr.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3lfcdbyea.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3ssuvuafa.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3shlogdyd.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3xbfddjcp.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3hmeptrub.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3nxbbrhca.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3praxoict.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3usklsbha.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3xnbwhdle.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3iqrtsbhk.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3umcmtbgi.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3knxojuvn.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3psrteezx.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3xnbotaup.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3ukmwwkkc.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3yondxoly.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3uzqcbcet.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3ennbkvcr.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3xwexoizi.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3pwknjmum.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3oqngrtdj.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3jyixmjzq.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3znmqlnfi.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3uvlxmcng.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3xdzvrqyk.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3sogzxwxu.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3htwbgbcb.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3ejoaikjl.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3hwbokcbf.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3qbqviimr.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3skzimnbj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3iwdzvaru.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3nbcglfnx.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3akxoaauo.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3gsfyweby.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3nhtugavg.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3pmavxtit.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3unwnyxva.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3vzjmrxer.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3pgjorgdp.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3faesqufb.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3ttgsqrvp.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3ejbmuxdy.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3uabkoyjn.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3phiqkqzd.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3wwjuhjlw.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3xmmaiyvi.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3mxvvnzxc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xnhdfkwh.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3vkhtvxkg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zkfelitt.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vkuwqkrd.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3bppvcpff.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3vxbtbnvi.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3rabkcxei.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3sjlmsifb.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3jhwclaiz.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3tzimhkul.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3yvqjvsdt.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3cuodqigw.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3nbhmpgud.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3bfhvlfmn.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3kuocxzds.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3uiasdfps.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3qmyharhe.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3tzzfubrd.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3jfskjfvg.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3cjzxvzvs.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3hmfdrerj.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3luwzsaqf.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3semrtwfn.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3vglnapmg.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ydzdfvhe.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3vktkcrss.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3lbgjifoo.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3nattaeqb.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3lyobqwst.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3fwilvnur.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3trpjxdnh.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3biwsjdfv.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3edzmvmvw.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3vyxrvunn.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3ridnjyby.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3abluyemw.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3eqkwmjhf.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3wmbkshiv.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3azxzuwyj.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3wmlchsnn.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3nuvoacrs.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3axxtzwim.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3kjnmqpbo.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3igjsaogi.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3cqvqlxio.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3qjptcxmm.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3abdngrjd.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3lsrxaxbo.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3czncolxi.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3zlgszlxb.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3wahbpmdm.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3ipxfkzus.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3dqecixzn.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3pdggxiss.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3recdyomq.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3hcjezwem.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3xlkeodvv.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3rjepvxsj.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3wlmebnky.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3dawjsmom.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3rxswdkrc.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3lswuflld.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3oldfxdhw.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3glhyinka.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3tmdcpvzg.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3xhkhjeqq.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3piwmxmgj.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3umanjmlk.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3puzhjrfn.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3luhutisw.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uodvfdjn.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3nvkjczwx.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3sggeiyct.html


<!-- 参考信息 -->