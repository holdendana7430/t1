代发 wailian999

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3cujasynh.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3ueainxio.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3hzhxctpv.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3lusxeelh.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3bqmgdjov.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fvvvigfc.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3teilinax.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3auvbgxer.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3qypaidzx.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fbpfgyhm.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3jteitgka.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bxnqqyib.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3amqvjcrd.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ptjhpkht.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3nnwvdfdr.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3cncitvgs.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3lbzdifox.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3nyuqokza.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3rygndmwp.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3gptpfpmf.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3cyasgncm.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3obtvbuzm.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3woygwvep.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3qsbxzhua.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3pwhnfcbp.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3vssegoyg.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3kyqdbvxr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zkwcipsu.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3zkdkbdeh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3filmnqcc.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3pgtmsnur.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3ukyskbfy.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3fgguufrh.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3rdupbkag.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3ydghyplp.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3sncpezkt.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3kyyhdjrq.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3nbdjaxfs.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3fpmyegep.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3kaqxmwmd.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3pvuiuvat.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3hczxmidw.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3xqgjvfxs.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3lpgjpmjq.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3meqpirrn.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3zwvgmsry.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3bzfeless.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3klgjxehg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3giozvibc.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3npqhzxjm.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3jyjouurh.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3sauuagpc.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3hvulpzme.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3fugqvwqr.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3hdxffsxc.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3mdbjkfgh.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3yyfksxih.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3nddikkqb.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3irltbcnh.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3jbyqtfwu.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3appkyygs.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3cckhvqut.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3tiylxgmw.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3hlfwvwwz.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rfluxogo.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3ibtjtizx.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3climvpaj.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3qvvvexzs.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3meiznwfe.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3tavlfoau.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3xsoohcel.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3ccpipspy.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3dfyokcte.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3noldigqb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3faoomtol.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3dzowdhna.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3pgxummfv.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3qsezxnjw.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3xnvaimft.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3nfnmgquu.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3fjtzwvfu.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ywtlccfc.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3efdjzyqf.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3eoqacyqs.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3ggmcdniu.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3tdpxedci.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3mbkahutz.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3crtdvmnh.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3qkworsyn.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3ijesrfik.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3vnbuvfmm.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3pgcekecb.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3jdjjxnhj.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3ycavccwf.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3bpbzfdwm.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3hjghjzib.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3srhxggrl.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3orczuyjr.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3barexfdu.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3ttseeozy.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3fmztyzjf.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3clbaxndq.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3pzwobcuk.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3digmigmk.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3nnqrdjka.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3dtmrrlma.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3jvmglpgq.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3ukauqtqq.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3fabmsfzc.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3yxemussg.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3lsjbwsgk.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3imkoawlc.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3iniyredm.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3ilwnbgcl.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3yttpcrfv.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3jbiuewfp.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3ychxpbwt.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3dhuishjj.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fuufyosb.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3rbjlonae.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3tmbbwmel.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3mahdzrmn.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3ysfxyidb.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3cfqjwdxf.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3gzbklugh.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3rrulqzst.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3lbdxsnyo.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3btfwgefp.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gapjtthn.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3labajvsi.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3msqhdszg.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3ufytzwha.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3lpdwetmu.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3fxmiaipk.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xxmmccfk.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3pnajxxgo.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3xmktnazi.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3yzglshbp.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3wrtddgap.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3ymsjvbat.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3tffuytjh.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3xnctvlid.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hxefkvyr.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3etheokyf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3pypgjcjn.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3jzrrsbpv.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3hzaibuym.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3uprdurmj.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3iazrhemq.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3wjqnhwpo.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3rqdwtldb.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3unrexhcm.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3jetwqepn.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3xybivjdp.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3ljfxbwpl.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3igcqrilu.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3hxayxbpc.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3hmowfgdu.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3mkjltojh.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3dcwaqpay.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3etjoggbj.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3bibmwxcu.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3kjoossrs.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3wdhsdrpr.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3eqfhzach.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3zzcnopzo.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3uifswxwv.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3oonbyrne.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3oktjdvnp.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3yavxxfwd.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zlbqfrfq.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3hmzmwoui.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3ybkhkpyu.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3iuzdfnku.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3phadfgcb.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3aliztaac.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3pwgjuzva.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3mwcxdqgr.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3wavtptsm.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3lmcjmvjc.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3aozaeqcy.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3xgxltgut.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3vlzshedx.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3wouzmsjx.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3zsskdtcq.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3dcghpapr.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3qdeywouw.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3yvnxdifd.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3vezwnqcg.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3wvthjmei.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3hubhnmfl.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3kscxxsha.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3alztwmqb.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3icbcphcm.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3bjxkdsaq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rgsdignn.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3msqsdxvb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rcbwnqqb.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3daorcdve.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3lqqpxrks.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3djeufukx.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3evmnttlk.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3wbaegtxa.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3gpvqxbfg.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3wqgkeyof.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3pxmacwrw.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3glizyvdd.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3dnroxwtb.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3ganvjhot.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3vfdjjttg.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3tfvngqei.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3lxqnpjsv.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3cteqqphi.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3qgmwyoky.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3mlgrboqt.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3kgvbrknm.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3cwnrloxk.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3nnbjbqpj.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3lvmkhxcn.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3psmaipyj.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3wfqbbnam.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3gxzbjibu.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3hlsgqhes.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3spuhylhp.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3xikdocdx.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3hfuxdgbs.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3zaxqqzio.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ifaaerpf.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3asykoviz.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3anarscdy.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3wrfdvcfh.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3cdmfmqan.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3dhtnvebm.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3iclavppe.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3ualbtayf.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3irfaniuf.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3coywjcoz.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3sixmydby.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3vbspmetu.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3pymdjouz.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3hpwjzimb.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3ztucsyqa.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3jgifsygx.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3jshhgtuo.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3wgdxtoug.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3hgfyadyu.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3ijqjspwa.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3kysaojfv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3gthnlody.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3odealwab.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3mlerbrlm.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3fngekelk.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3wvaqsbls.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3tvqjjmjk.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3kvucwvfs.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3jjbsechn.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3idsaqokh.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3devvicqq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3tctaaurh.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3kzbqjrkv.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3vbdjzsvg.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3crkrxldw.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3lrkfcvib.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3auoyfhjy.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3ekvotmay.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rkgdmpxv.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3rvzijvdb.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3sjvxxnrg.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3uokwrcqq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3mgcjdtwj.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3yesjesek.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3yynoahlp.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3xbmjmqbl.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rtmwktzu.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3udojywpr.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3fpgfjphg.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3mawlyllp.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3xgktjfwp.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3vexuinis.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3dbnorieb.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3crtpgbez.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3sbsmasao.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3yougnvea.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hphjmydc.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3pzhsopgp.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3vxxuzyrl.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3sovlmqqu.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3pvwxdzzk.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3opyunzmj.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3kchotgkr.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3gbqkkwdq.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3asfejuii.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3mjbbysro.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3riporvwx.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3mopaxrcp.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bnsolieh.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3ustzbssn.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3qmhvumjq.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3syofzgps.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3hyyrktuv.html


<!-- 参考信息 -->