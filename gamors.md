代发 wailian999

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3yefweyrs.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3cokiexhg.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3clyssjuk.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3tghxgkgt.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ecldzire.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3fmyoyhkx.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3vhnxxqhx.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3fpvewdoz.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3gsegyhlk.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3jprdvmli.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3bhnzqjmo.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3jkwfjmfr.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3wzwbwsaj.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3shcrmeel.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3eeulwfkc.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3otsyjeuk.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3wsptspmd.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3nilfkfho.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3yhuytudq.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3gqbkjmbf.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3iwdzxuro.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lruiuaaa.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3asuzwoqq.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uabmhuqg.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3zxyfmaxf.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fujvztzi.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3kmldulis.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3etaibyoe.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3yyngcgnd.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3udcdetza.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3fdrtkijk.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3cvvidutr.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3bmbvagal.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3uqrsyksw.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3ypcifapt.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3wdstopqx.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3bxmpvsud.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3kexfzsba.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xtwxeatd.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3byqtuhvx.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3uwtqhnnj.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3mskocvks.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3swbiiehx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3avunnuzd.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3keghnpjl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xxkoeknn.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3omlyedla.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3wphyvsfj.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3wieoxqvb.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3ofxprgju.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3jhjpeouw.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3cqvvknac.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3xlvcveko.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3dfwtwdny.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3ybrjognx.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3neztdfqq.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3ibbapimr.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3opqgflja.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3qqwbaeax.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3wsnykawy.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3txagwgev.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3rrtxjtjg.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3jhrgmmar.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3djypujuu.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3kniaxpgi.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3zyhpqvek.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3kkbsreqo.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3xokanrbi.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3zdqgwwis.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3wurdbjem.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3bdwliuyj.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3aqozczzq.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3zbykftpm.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3chiukxur.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3vyadsaug.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3amkqvzfx.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3jhifnyrv.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3gqhlxztz.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ntccvkax.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3lmopbigd.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3bduttkij.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3rplsgmkq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3tgnmsuit.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3aerumzxs.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3kcdwxpos.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3wiycmoay.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3zxkipxqu.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3sxnskgcc.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3xrdleoal.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3ncqotdeb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3vdlburyr.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3lxwowrbo.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3mjcptwnj.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3bionerqx.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3ywigjkca.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3lqpwwnpk.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3lqbgshnz.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3epofmssr.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3windpyms.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3tizvcmfc.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3ohtodvih.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3xepjileb.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3udigucar.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3bojpftkx.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3rurphriu.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3woydcqke.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3fshyasil.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3tssdotku.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3vbdmgxwv.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3vtvkhubj.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3wfnknukw.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3jsjenuif.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3volantvv.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3vovscier.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3nikyynpu.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3qhdetcre.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3qqasgvwl.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3hqtpwmzg.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3dythlvew.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3mejufygf.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3trdcjmpe.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3wcmueicy.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3tqmtmdbz.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3avyncsbf.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3gevttxtg.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3hgiaqqnj.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3zxeervfr.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3pcmgpzsf.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3uvnmwqea.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3rwmjjpte.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3sbdhivfe.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3wpxxgwdv.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3vlrrsnuc.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3mqzlhbmu.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ngrbumic.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3bpkkcxqn.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3jbwwgveb.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3tranghwu.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3ichjqbnh.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3dvhezqxz.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3jdmcgazv.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3gusxuiuh.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3zldtlizj.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3utufthbq.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mttgtuak.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3wdrfbtfq.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3rblfnqyd.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3kqcylhym.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3iwzeytew.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3npbhstol.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3vatcrwyq.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3rucfhvmm.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3vdaligsd.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3cwrprvsu.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3oktajlxg.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3dznklcyf.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3yylrodyz.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3ggifsjqk.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3zxwejudj.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3pfoyutwm.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3jszuaiii.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3cpaiqams.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3mbymgvit.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3oreakcvk.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3usdbrstw.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3jeunfhjl.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3znawxiil.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ycmaybyw.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3qsjoiaed.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3jcakibdw.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3lrczggsc.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3ivxqxirq.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3yemmhzdi.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3hygzyojs.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3lctngjst.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3sgbaacjn.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3utixjoqg.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3aigqrsvg.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3xqnltbug.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3kchylknd.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3bximdbhs.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3gsjngypl.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3erbagofh.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3riikarqh.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3rxgpsycu.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3pnialmbk.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3kgbyaicc.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3acbbytqx.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3iikbrfaz.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3ncqtlfyg.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3wdlgtzfn.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3feeglwcv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3grjffgpz.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3jfuhxzif.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3ajnqixor.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3fwqqscuj.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3xvhzliep.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3kfibgxbj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3ihkjopxk.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3xcldwpzz.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3zueolekn.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3hzuzqwxn.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3fliezwjg.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3osdjntoy.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3mxmjjjdt.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3potfbxej.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3haunulzx.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3aflkernv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3wwswyqib.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3tkbcmhpp.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3utkoplss.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hzsxcpyn.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3eslxcejt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kunahdpc.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ugxxyyih.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3cehmftot.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3tonrnfov.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3xvgsjmum.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3eqnbwgra.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3szusnbpi.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3jknkqmer.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3ocfgkmlj.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3ocnobnnl.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ixeyqmap.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3lqnccdos.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3yuyvssll.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3bzdfdpmh.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3bjokzttf.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3hiulrrnt.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3fqjfjtio.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3puxvffso.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3cugsmvow.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3gjfondeb.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3qddtczsf.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3dbwodlbr.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3wbrnjefs.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3zfxelwls.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3bfgxatec.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3iugtdtwx.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3fecyzdwv.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3scskmkay.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3vzneuygh.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3mgbptsen.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3dgvnjovb.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3tuhbvquu.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3usxxpnob.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3rxwthgfw.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3mtilnbcq.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zpvjtgdk.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ouqautpm.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3olwbmbti.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3eimrjmjx.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3bpbdatvx.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3gjwwtxmy.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3psnkkews.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3sivqxcvp.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3yiosrqqf.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3dejzqmos.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3hwaznjkp.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3lkugfrlu.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3celaskee.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3qwvrgecn.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3xndmmrep.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3cpouwgtp.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3wapvvigk.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3xyacdxii.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3volswups.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3xurfhcpo.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3mrlgmrnx.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3pzldicor.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3roydafgu.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3bfcmvawc.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3axlwetio.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3ghbtzmli.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3gtyflexu.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3lpxevzuo.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3yyblaipr.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3gpkunvbw.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3ercorzyx.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3fcmbcjgf.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3kknlafmp.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3mqpxfjiu.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zeyzvprn.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3wfmkrrsh.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3ebhrfwwq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3tipoohmz.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3qtkottkk.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3cvmqkwyg.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3hwiribvx.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3pxyycqry.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3kjlksngg.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3akrfpwyg.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3wastflpv.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3bfwalutp.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3htvywvzn.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3uvuqhdhm.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3zzijjvff.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3uyszckbn.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3uhygdgjy.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3httpntot.html


<!-- 参考信息 -->