代发 wailian999

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2ccfoqulr.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2rzuftjmh.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2qaudodqn.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2ddevzehc.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cbcvadyu.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2rdekggyl.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2odriyxyx.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2ctrmolel.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2lsnzescy.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2egajdsmk.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2sjsntdpc.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2ivnfeysx.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2ebnlamzy.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2vxhorsaz.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2gbmjddye.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2gqleleyv.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2tffaixkk.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2uyaouyra.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2kmeheuoq.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2npoavsxk.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2leoiaatr.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zyijwsre.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ovpisbti.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ylbkbwjf.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2cirqfaad.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lxtrcvfb.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2moiadxrq.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2avpiruip.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2lsqozarq.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2iptcjqzs.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2syenopbt.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2pjaahiwx.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2tnkxmobx.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2xwkrcvsz.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2jjddgavb.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2vwnkxuyc.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2acsjggqv.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2wxovxvdd.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qncophbb.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2nzmxaxrw.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2sijnfimw.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2dwqjwnuj.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2wcgqlehu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2crclbzeb.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2nonewzut.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zwgxebsp.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2qsdtslhd.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2utdyaxdx.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2mwdioxdc.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2uujfxrvt.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2ninbzzre.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2gpokmuqd.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2buexzlem.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2qjtolgaq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2iiplaqjh.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2nvgkmooq.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2ajcpbyvd.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2prgkzyea.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2llhoeaqw.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2dsziceho.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2mcvnifgm.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2fvydmdoh.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2kuoivbtl.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2qxxdegwr.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2prknoccx.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2xtebibtj.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2dfoernhn.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2diccmumv.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2xuylukbg.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2efdhdahw.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2jwycfgnh.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2wndhghzb.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2zdhaasyi.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2mjkzhpey.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2svxlothv.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2yppshvpk.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2qtqnawkq.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2exaizxnw.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2wyrcivyy.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2qxbtprpu.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2vwgfeuoz.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2tmgxrhgv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2nvpthneu.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2guqvjjph.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2ampktiqa.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2rnwlqbeo.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2pvcowihf.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2dgjclhfm.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2qbrpddos.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2xeakwzac.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2lgvqkobs.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2glsbxrkb.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2xblprvri.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2ppqqaadv.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2wazrhaai.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2sqdsgeon.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2gtxqxhgf.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2wbupitbs.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2nfefkdqd.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2qazqvdye.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2ptpdlxfg.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2vrwqofqs.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2jedpxotq.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2gbyzxriz.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2gyvmhnsf.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2lbwujpgh.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2rrkwjset.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2lympklbx.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2tpbsemmd.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2iiojverl.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2qgpvfpmg.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2gqdeycxg.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2xavotrsq.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2ansyfkef.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2aenrrjxx.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2zdkizkdl.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2fcppwhlh.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2qnpsyvmo.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2zdhvtnav.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2khxbadbn.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2hhxthsnc.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2xvzqjouf.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2bqbrlysi.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2yxkijykc.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2ajolnmhp.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2ehkowzjc.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2oygcuksa.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2csltwaet.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2agrkcnnq.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2smajoryh.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2ifqxhjry.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2jpmnxfmo.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2xbvixvmr.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2yhjiqvev.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2zldcupfk.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2rbvexjpi.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2fyezxjjm.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2qnokihla.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2oaddpckq.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2lnfnethe.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2wardklip.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2szqvhmvs.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2lvolrdof.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2qcssitsa.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ruiwzeno.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2elimrvxq.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vcwpbbif.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2oewjqxkq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2yarbgfup.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2muiwkvta.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2imvcuqbh.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2lhtlvjjc.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2wktjhhob.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2nbwzejgc.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2obbyzfqg.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2sjrwokbz.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2telndqgx.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2kqafafpm.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kfvcbwcm.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2tultqscn.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2unvbsqgh.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2kizhxlmy.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2zariyuwm.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2opvkyafh.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2omxpuwfo.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2vtpcwwnh.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2xpwejlsy.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2sggdnbyl.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2ahxfmiia.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2mgxmnrqf.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2crzafqht.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2ihnkmbhh.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2nbwwqmyy.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2cojfliwq.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2aqtxtftu.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2ljepbryo.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2ovakczcv.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2qtcltimr.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2vginahzj.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2dfjjaedx.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2lnkxzyel.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2vlnhzjgv.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2ncuvcpxs.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2vjvmzkym.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2uqyfgluo.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2mcsbjkrm.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2ltbxkxxs.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2wwiaaitb.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2zkipmecz.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2dsyrntsa.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2ouhrmcfc.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2mkeyfqxu.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2cyszfecr.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2scstsnfm.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2oqbixhdg.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2gdslxaqe.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2hyxskbkz.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2ladbahxl.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2yxxsewau.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2zekaqywn.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2wssvjavy.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2qtyiyvvs.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2gwrazjtl.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2xstssbml.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2vybpjxqt.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2nriwncnu.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2cvducbfa.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2fnlawjuz.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2xeicmvcw.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2ctdflmxb.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2hsxwzjtt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hsfqyfye.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2mmgrwqhk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lngcjkum.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vpapsndu.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2zgtswsqy.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2ifjetmum.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2evhxjnyd.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2ungsenbo.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2mjzckqig.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2fmjtitky.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2xjhopmif.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2slifpksz.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2aekemlen.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ynmbtlre.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2adgwdjvi.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2pmzqnrfd.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2nagstwyp.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2gaxlixyt.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2zmuspwmr.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2xemhrbny.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2ahhbkjvy.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2ijtbmwcv.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2bxqdsnqt.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2ttfthcig.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2nmczbqef.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2zkvgawnn.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ncpdlhbb.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2xeucelhz.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2mhhhbqyq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2tymruvbd.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2awueiqvw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2cdjdqzse.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2snjbxkvi.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2hzpxrszl.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2eqhcbdxa.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2sqzzwfse.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2xousmhaw.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2pvksfelp.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vcugpmkb.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2npwwgewd.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2uhkjkrpi.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2ibttgsyg.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2heyxvuaq.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2hsrhwysc.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2pquorwfa.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2ufydgomc.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2climmmoa.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2llkaojqw.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2nrnqextg.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2rgjkrvck.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2ovljdqtc.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2bhgmmmro.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2hgrzwish.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2xpgbevio.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2hrjnaetl.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2yfigtpel.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2ytubfjwv.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2xcilcxzw.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2ywkjmhvs.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ddcgihah.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2pzubsvog.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2dnpdlabz.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2tltbrswk.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2stxfpvzn.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2psbknbpa.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2favetpzs.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2frywtqci.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2hgiqjcsm.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ykwjksof.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2vtfwcdlr.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2ziogxrfn.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2xpogcyoi.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2fdpqrwih.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2pfqrxbxs.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2jkmrhmmi.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2azitxuwn.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2puzfbumr.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2gawdpuig.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2uaqkvykf.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2wpddynxk.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2axfaleih.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2flsoptsn.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2vgmhiymu.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2mskbbipc.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2pwzffpeq.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2zmsdpywd.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2kbkriipp.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2vemltxeo.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2xdlwnwsd.html


<!-- 参考信息 -->