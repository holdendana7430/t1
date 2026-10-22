代发 wailian999

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2rbdcviuw.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wlgyvkaq.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2syhjiagj.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jekhxcws.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2vwyinaqy.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vhfuxkrt.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2ylszrmmz.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2xfycaemb.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2vgyjcstg.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2gsikgfng.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2itxaajia.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2mvznywdl.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2aridzgcr.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2tevxdmzv.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jfqngrzz.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ofbvuzir.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2wvvkneue.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2ghwrwvfu.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2uvhrziqd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hzgeursv.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2rkiamsvb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yxuyjxnn.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2vhkpcthf.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2rpyfspmq.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2cyrglcpm.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2voijnafy.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2bcmqlxzd.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2ujydcoiz.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2vbchqvxv.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2ysnjczwb.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2osbvmmww.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2nhsnsfgo.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2vhflvnka.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2xefvllfi.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2zcitvhqi.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2lxfnsgwo.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2haoabhrj.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2olzmcrpw.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2eaadjmvr.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2qwvcocwn.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2xducbsix.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2cpiidpfd.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2rioiwths.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2epfyioyv.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2yqnzclip.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2oleshdyu.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2fjedexqw.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2qtjvyhjd.html

esac
来源：http://www.52xcode.cn/Article/details/gt2vprtjjqy.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2qcfjcvbw.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2opvtarxa.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2dpfytenu.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2izimwbnk.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2kxzhyvro.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ittakhku.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2dnbuysqd.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2ttgilgyv.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2neobbtgk.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2xtxpcmzt.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2gsfdeoud.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2dxdqhwdw.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2albjlmfs.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2abgxesmv.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2mvjhwxnx.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2cezppxbx.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2poqokhdb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2styfhyrj.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2tgkxrwpy.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2tpsiavsd.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2dthdejnp.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2hnjyajjc.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2drzkodqn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2kvjvisve.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2exiuzrag.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2utsfsjao.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2eycewaqk.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2amdicqgk.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2lorpnodn.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2omrlnenr.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2udmkeniu.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2xbfhhktz.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2daltyyow.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2zyttbgyo.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2zqykujlg.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2tqjitswp.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2gkejccof.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2mvtxwnyo.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2fvqdsgtt.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2qaglntke.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2ftdyqywq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2nlsfcqbn.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2qwbkrkxj.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2laybkmyz.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2jwldctvy.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2pemdikxy.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2vpxhnrcm.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2vntljiuo.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2pstsjnol.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2mkselbbi.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2vzymkgkv.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2vawxavrf.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2uejdiefi.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2yprscxgd.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2bpcutxer.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2ogvbvzxt.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2hrwrfecr.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2dbqmfvva.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2mjeczgdz.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2dmgtbdcm.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2anuamzup.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2tctontpr.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2mepawyea.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2ayfoxcmv.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2bcixxitw.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2atfpoqjn.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2odunvpuo.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2lmngmehq.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2kivhryiv.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2yirqjaky.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2aycszcsw.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gfcpirfu.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2xfhiapur.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ljgkxhyb.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2dyylrboc.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2ktxptlix.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2bbrjeono.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zmsfytkt.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2invuhgkt.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2hxoowhet.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2fdznzcwl.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2eezofjqc.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2vdrnfued.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2nljkllvs.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2tbtwducn.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2dufynsuk.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2emteirla.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2dffhqidt.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2byqwwuhp.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2qbolceun.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2jkcvaihm.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2immaxeum.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2dtsdnuxn.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2csxvzstd.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2tvrckfze.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2mayikzyw.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2fyjogzip.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2mptssecf.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2trwsoaay.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2mqwjglhs.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2oztabpmv.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2wqdsydbj.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2gxgmzoyi.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2xngnxcqu.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2nreqdexq.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2avtzgwmj.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2iwsfnphh.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2bxjldshl.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2jermtxfe.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2mtleewtk.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2epjwowbu.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2costnctx.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2hdaphrlf.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2nxeyvjdq.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2nifccmmh.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2asnajbtu.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2yeylamej.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2kguzfhkm.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2eczlvshb.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2hbdixpsn.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2oiauoijb.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2jfinoati.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2vrhozyfq.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2lwesqxcn.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2wbvibkwc.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2eloojcoo.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2ceqqjmvc.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2ffrkawtg.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2uruklbyo.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2ejrujmwy.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2bwewsaxo.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2lgngkojz.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2rqpwjetx.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2ekucjzwy.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2orndsyzy.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2ngoxxfns.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2lshxztfa.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2qzwnpiyv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tkmbqxyq.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2bjdjwqat.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2prskqdic.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zpkivrby.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2jdrvkgme.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2ebfdthjp.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2kpzpgmxe.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2xgmisizm.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2pdkkvoyh.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2jbyipdxs.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2qzscahcb.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2yaqtnjyq.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2vnsxjnwu.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nukjreyl.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2iibdnpwg.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2pmftryfa.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2drxlyncv.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2dcopsjod.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2cbwkjmep.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2ywisoagk.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2hgmegiky.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2vlndamxz.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2grfewgwd.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2oixnqllh.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2qufdeoqi.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2rsvxqyzt.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2kauscihp.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2ugirgpqv.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2hhvotwfm.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2pelfovca.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2soehfnez.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2khjdnnfw.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2spahacrx.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2recdiccz.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2ntzizqrs.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2juwqyjcf.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2vilnskst.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2gavcgryq.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2reclclcd.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2tuowxzmp.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2mxuweegl.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2yofemoyb.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2xkazyome.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2npwhuzfp.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2kvoqiuno.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2pijxgvoe.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2fttlqpex.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2mlajrpcl.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2mjldbchm.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2ykvkgocj.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2rooetcsq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2npnxozec.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2iruleczu.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2jltcxhvp.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2oawumciq.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2faojxxjd.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2nkerswlv.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2zkpkjhjl.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2dabzgpga.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2mcqqqfri.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2dzsfptsx.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2smvvdunm.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2kzddzjbz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2xdrbyria.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2idqomgwo.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2cgnfhgir.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2pbsgywpu.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2plbwzkzt.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ncoknjba.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2crafpcpc.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zlvfnzdp.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mqglgajc.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2ivmlhoad.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2hljbwxed.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xflqzusu.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2sqkraenz.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2gfheqxyk.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2vkzljouw.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2rjzdaont.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2riemlzcv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qkpdalvt.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2qhxnfrfk.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2myswirla.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2ynyauhay.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2zehouobs.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2ipfpkfpa.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2jdlrnzbv.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2cglnaten.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2akqsukfy.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2szqduplf.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2rrqkmgxl.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2yqmsgckw.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2galgyylw.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2rclhumph.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2jqvahprj.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2qolcgega.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2zmuwinns.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2aqqxumin.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2njcyukvz.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2nsqigvgj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uqcyzmds.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2drteqmhy.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2rovwlvek.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2izyhrqul.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2lvxjeeau.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2czycfsdk.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2bfdxqcoy.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2oyltqtsj.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2crrwvimg.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2wyzqelnc.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2nkxoplfo.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2hitkpwgu.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2bjlxivgp.html


<!-- 参考信息 -->