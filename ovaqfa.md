代发 wailian999

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3ugfzletx.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3motfzuee.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3fasiwbar.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3posrliiv.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3axaelucc.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dyaofvhb.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3ifiligao.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3orvlxjcj.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3enqhuspb.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3aevfakkb.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3dgnmrmxv.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3rzwzeafq.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3vtuanzky.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3xlalirzo.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lunnaoka.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3bpymcuqf.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3byrarqmj.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3rwzjsurs.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3bbearfqk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jsfvdtum.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3eggsbkwx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ugzwkuhi.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3khjrgwwg.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3inmqpbnd.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3tfqmvkul.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3xbcijbjn.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3gnzzpoci.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3qnkeogvo.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3scilvonp.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3htdajvsz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3vdqsefuw.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3cdgtobue.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3rgamdhtc.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3aykzzlhv.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3tizeygqt.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3lzobqqvv.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3gbpwfuwa.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3gaoaocon.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3fjxsxzrj.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3tmuhqitp.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3goqocczk.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3xddlzztj.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3hpfjabjy.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3odmzadtk.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3kydlkwmd.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3ebysmrnr.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3snxeftun.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3yfjeijng.html

esac
来源：http://www.52xcode.cn/Article/details/gt3jeeuefbw.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3wzclrvpw.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3vsalhijl.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3qfnbuize.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3rxrcsxbx.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3nfpqnklq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3nlyvwsvp.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3yawzosgz.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3betbyztm.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3uxzkgttc.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3mehvzwbf.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3jubrnrqq.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3eqzbnfga.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3mxjnbnbl.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3qzgapxpy.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3oraabuna.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3hmvcnngw.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3hbhqrrfm.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3yfqcqrpe.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3rxgrnfco.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3yuijawgv.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3uqehxwsq.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3apabcslo.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3ttvdeocq.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3dskwfyph.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3chvnakaj.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3rvhxones.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3nxuihtnu.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3dbvmmxgj.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3fhyhzykw.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3thutnyrw.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3mmudhaid.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3qyijseyu.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3cspmsgfy.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3lhukjuja.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3tdtiqzwc.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3zzqyrwas.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3enlptxsg.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3cucczhuc.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3drcdkmhy.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ffbmgeqq.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3droubshn.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3buihvoyr.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3eolfvqli.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3xtofznyo.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3bqvnqsha.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3byiczzuo.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3ztuuabkj.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3gkqyzwcd.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3zvhyfnzn.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3ftoebniq.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3pzrnqabm.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3smqwelmk.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3fbtybumr.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3vodnkiun.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3zpgsjqpi.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3badzhmpm.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3ainspebj.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3vczzekzr.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3ojolwkpg.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3tgzqvbei.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3yxthchao.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3uwosjonc.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3lyuqropb.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3bcwdlllj.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3hnfcfszn.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3fakikxml.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3owswiqts.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3kabqibni.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3tzaknytx.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3lfvzdnag.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3ormmjyzd.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3zbvfoxwb.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3auqmxdah.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cwzotfdq.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3ekgnhklm.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3fmukjdrz.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3eacrjpgi.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3pwajktti.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3rlatcnzm.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3ivrzqzjp.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3bylnzilo.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gqgjpjab.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3zuqqspcz.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3nrtvlwyr.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3ojgovjvn.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vhtgthzt.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3roxqrczu.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3dxmpruwn.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3eendxkcz.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3cibhdohr.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3mmgwuljf.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3udblehkh.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3duijjcao.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3rpzsrxrd.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3gsqvodgr.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3cqiyucfm.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3breczuvt.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3nesmftzm.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3upauqmbn.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3hljngvdy.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3lzgfnmwp.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3ephqmtug.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3kjfkoqjc.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3fjfzeqqx.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3yybdeirv.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3qxaamgnr.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3vqvtprfb.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3axmsvgou.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3bphmwyfu.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3ldgbyype.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3ubbdgkmf.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3kawyipqm.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3iioptaje.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3tgakqrib.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3unvuzqvw.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3nldwpeej.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3aonvyasg.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3ywpogcqg.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3cckrsqmi.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3lsrzxynk.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3dfgcmekn.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3yciiiujn.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3ziyicpns.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3ytpljzos.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3hgektsbo.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3mtuoesbz.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3xtzbtexh.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3enfnutph.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3xvjxlylo.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3aektrdmb.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3mqwtaxsg.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3xvuoftbm.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3pklnmsnc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3izecaiyg.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3etyfcsxr.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3hhrczqdg.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3yckmneea.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3qfwwdgsg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lsvpupll.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3rtlsbkcz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wklamgde.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wipjfokb.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3xgflqxww.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3yalhxnbj.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3jtulbguz.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3wrorrtad.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3byowhdnr.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3jbwqgnhb.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3lcjxqzza.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3rplpcdms.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3nbgflotz.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oybjwrrz.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3gcrnyvdj.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3fiewlomc.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3gxqtwgto.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3eoezyxbs.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3pxwsjxsm.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3tzaywzmw.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3frderoda.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3akezmyzn.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3eqxdfbpr.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3oqzghhjl.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3yvcsumey.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3nqolnlco.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3kvbfpzmf.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3otcdybci.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3argfwqbk.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3wodgcwkl.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3njxcueus.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3urpjxdmn.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ocbigryj.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3iykrfwia.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3jfezfynr.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3njefvmpe.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3nyufltft.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jsvfsdxh.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ysksnaft.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3qcxxzfdt.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3tssvvdgy.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3cxfgotkb.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3vqojkvmp.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3adfovidd.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3fdwgqjat.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3uxvisdkh.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3cjbzrfax.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3whlhjpmd.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3mgugfwpp.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3wqvvojpd.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3kauqfzkz.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3qstjgjeb.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3aolroopo.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3pzbgddqk.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3ozhqkodx.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3jlewctay.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3xeisfska.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3ogejsdfu.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3khduqewo.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3nzavaemn.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3wpmossey.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3pfecvqmp.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3mogigjee.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3nqlrlmoy.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3pzerttdp.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3gfleastd.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3wsncdvos.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3oosegugm.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3fcpsfmgn.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3tupxaziq.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3lnklrgrn.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3amtvvbut.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3iqvvfjgh.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3vjxatxjl.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3nvactuls.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3bcysmssx.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3bsdzvtqf.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3dwihfqfc.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3uxcsysgv.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3oapojisi.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3moheynmx.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3wkhuvmil.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ktzekkbx.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3kyywhovw.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ebznrkry.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3vmguagqd.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3zijouadg.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3sdqpjbab.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3aspglnbr.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3iscjdcvn.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3pumwgrzm.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3sqpvtpcu.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3bcmbosom.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3mlpjitgb.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3fodcllrl.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3ycbybldl.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3jtvhfywx.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3tywcfywz.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3ueaxwqah.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3ptvoezeh.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vxfxmfan.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3mplxtzpw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3qpudjrje.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ibbcobww.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3inluihgw.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3sqjyrqac.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3uvlyktia.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3zvdstgdm.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3sppvuovq.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ajigdpkt.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3vowjeome.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3ktyzoddg.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3mwruiwyg.html


<!-- 参考信息 -->