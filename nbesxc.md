代发 wailian999

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jklhjtio.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2eulwrugf.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2scmzzaae.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2dhalcoxr.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2nsoqgaap.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2fqroorhm.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2yvatlseu.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2xlfweagf.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2tnrfxjhy.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2uzfxhgwn.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2lymqnozx.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2njygsqjh.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2rqsdkcqh.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2qmlrxsts.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2pezdkbsv.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2gdneevbv.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2fccshzyo.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wprwuabb.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2ehhwtzus.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2aarwauwo.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2bnxedmyv.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jvccduke.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2sgduqlmn.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pyyyyypc.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2gpplfeqn.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ryfptjdz.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2bvhvjxdv.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2glxkqziy.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2gynzrikn.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2gwbeuhgj.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2cazuhrro.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2khefbqwc.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2loztmlii.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2pkstwxbf.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yqwskhgb.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2rdjyttsf.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2bjpvsbho.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2zutmroig.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2thslrlkl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gwaenasw.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2dxirijkq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2txverjdi.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2jqksqdhp.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2mpmomegi.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2cvsrzdyl.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2yodjvzmm.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2hbkuwwki.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2bkmgmuqh.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2ajqezjbc.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2fwybudcm.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2azohpuac.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2itpnmdnx.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2depqvxen.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2uczbsmqt.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2fxarmnsn.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2llqlhphv.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2yvrbovmr.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2oxkzifha.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2qinvzcrg.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2xdoomaqq.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2ypgbvrhy.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2lqcjzbnb.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2zkbcqxsf.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2smhdhfcg.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2pwqvqpsb.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2rekgmtdc.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2tusdbtgx.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2zyszzoda.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2vrpqsxcm.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2nwrvxotd.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2aloonbgq.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2mxmmztlo.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2uicfqdgj.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2yqkkfqqo.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2goadsrxe.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2drvtzpva.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vlfobsrg.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2qwdpjmrx.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2eybbqifv.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2vmgfweft.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2sqasyuls.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2sopnmczc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2httldjrq.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2vvnpcycx.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2lmfxvjqw.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2hjnhmnkr.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2pwkjhscz.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2dggthdcq.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2bbdiemsy.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2fosijavr.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2auukkodh.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2gpmvpkwf.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2pkveprci.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2dgrgtbny.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2aostswdw.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2mdtcswhp.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2xnnjmnwy.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2kgbeiijp.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2klamelux.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2mnqlbtsm.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2zuecnvpn.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2yobkixqy.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2qdtbatqc.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2fblywjwn.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2glfkkpit.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2bfpgpzxq.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2gngwgbnw.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2esykiywb.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2qkpdqjsg.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2tbxwslej.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2yvynykte.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2saqvdcvu.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2fxbumvpc.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2skhebgfw.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2tazhrpvo.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2ouxegppz.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2druljfxy.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2hlpkzpft.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2eccovvfr.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2fvcunpag.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2fzbyvcug.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2sgbrfmrf.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2twxjdwwe.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2zhkbzyna.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2cnhopxfa.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2iroizikc.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2sgqjizjx.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2lttkgmfk.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2lvihlbyb.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2kxnvlzzp.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rufuivrx.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2nzyqrchp.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2epgfqefh.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2zbrgruik.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2sfdxtjee.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2ugxjjmad.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2cnyvjdim.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2ionetfyf.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2kolmyrru.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2wwrerwuo.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dzkqcvqe.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2gggbodaz.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fyslojvo.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2taioafde.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2nfofyflw.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2pdcjpsao.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2qtndoflg.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2xtklhrtw.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2qxpqcffa.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2sexpwxgg.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2nuizrqot.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2nlcwufom.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2rgsbtzrh.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2ywvnbgmf.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2enblzwib.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2saybusqn.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2iraofaxf.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2gxswargv.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2vmfrbijg.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2ofnaxplu.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2azcxaesj.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2dknbyptz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2cxksrcux.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2usjfvuti.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2uhvoitgx.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2vlwldbyy.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2ewfwwsdm.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2ypocetrz.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2lrseqcbs.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2gazdcmko.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2oucfrjmp.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2vhndpfjs.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2zpxtmqdl.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2dfiteufy.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2fqdfqqdd.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2jxkqoxfo.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2ecsovwbr.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2nmkhfexk.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2pnnsttdo.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2kfptvjbu.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2mjpyfzqt.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2xxfprgpw.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2efgylwjb.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2uwpagonf.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2pbwzhjaf.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2bnlqafys.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2umdkordq.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2wieikkkn.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2bdncqpup.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2hslyydsm.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2cmjyhnmk.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2qwftzgwy.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2aphjjtfs.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2dytyahyv.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ykzaleir.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2ujrqlheg.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2itackmrr.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2lticsvzz.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2aazsjsad.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2bmnowurt.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2grcxmelh.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2qjdgshmw.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2dwolqlly.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2khytygak.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2rmnriktc.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2bupnmnjb.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2rrawqpfl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mjfnwifh.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2mwfcgfsn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2evuszwrs.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tfzvjscv.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2wuhxjcjq.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2rhwlkbke.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2lfavllrq.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2aorkjylz.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2tscepjss.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2cmyrptuf.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2ahnnboeo.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ghlruppe.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2vwuitsty.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2sawgyeiy.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ajresjtg.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2ehreamxd.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2hdawktzw.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2cezwdosh.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2aavlgkzk.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2xijtggmw.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2vzdqmuyp.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2kkjpcwha.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2azvmhifn.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2cbulemqx.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2tjzmwjwi.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2nejqglne.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2zieiycyl.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2esxqzbqn.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2iztsukoj.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2pdmlzgdq.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2vgcpebgo.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2sejkmjdw.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2rwustkvs.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2xtvihave.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2fkygjlrd.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2rhhllhbb.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2aeffvvlx.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2gfrnzkju.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2vybgkwka.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2wfxqyevf.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2ktacxutv.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2otjfavpq.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2dougylsy.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2mfsrvgbr.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2rpmsgbvf.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2mdoohusd.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2rgsnmnpy.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2osomxlqg.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2xekszdqf.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2tchoqfzq.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2nnnrikfq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2nufpawof.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2hwhoslkp.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2ibxmznaf.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2cctiolgr.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2xtfakxfx.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2dfrionqr.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2kjkwhglh.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2cotuinwu.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2cbqjihpr.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2mfmprvld.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2exrhypbx.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2zmqqjerr.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2nzzsuuof.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2lbdoszga.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2gyweryii.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2izzxgimd.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2dtplyqmm.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2fonskhkt.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2qtpafvtn.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2didgsigm.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lqmmekom.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2covzyeqc.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2eqbfqilj.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2vmpeumwh.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2jvgdbpgy.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2ctnjkrmr.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2ttpxoyzd.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2nrcjcqlz.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2ajotrcnp.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2evwejeun.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2epxlomdr.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2nihwcujf.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2dhckykwg.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2mqywuxwr.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2oncwzwpi.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2lxjercee.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2tjnvshlg.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rveovnex.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2vayblxmy.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2kfuvfmco.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2ugokfbdu.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2vxhrptii.html


<!-- 参考信息 -->