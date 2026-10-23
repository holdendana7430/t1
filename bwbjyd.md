代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3smenxxgk.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3lvpoojtu.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3dylutunp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fjbfiybu.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3ymsgajwr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hyetxgsv.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3rzacmuih.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3tyegfxiz.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3flqhxeuk.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3tlwnrxcf.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3utvhcscy.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3tyfjjqhb.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3irmotnop.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3jyanausz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3hfydqhzh.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3vqbdigmt.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3yqhghurp.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3wyjygwtt.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3ehjcijuw.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3kykzvmpq.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3ozhriqfs.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3oscqtykw.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3urmritjw.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3gxsrzrvs.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3gaqngfka.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3idhurlzm.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3drlqhzij.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3wwiunham.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3ppsapscf.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3whiobrwy.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3mepjufqe.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3ssmqugco.html

esac
来源：http://www.52xcode.cn/Article/details/gt3rvvziuds.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3igjpvlma.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3kzzshiaa.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3obnopqmu.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ybwwmfoa.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3rzrnxfca.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3qbfakixv.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3wlevcjlb.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xrvhzljz.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3symdsboj.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3mzvrhxfl.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3nequqnmz.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3nttlprjs.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3rllvnjfe.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3lhzgkafx.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3qykgphtd.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3mfqcieis.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3wwiwxjvd.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3kksgxobr.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3awdkgtnd.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3qdcubrie.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3zxkvsdtn.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3ytncbxyg.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3amnikqau.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3hxrrhzgq.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3qmrjexkm.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3mayrwzln.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3thegtudx.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3oejjcqvy.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3sxbwiugx.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3jgopuoks.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3rysdtyro.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3xahtdfht.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3ohsrjupg.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3cxakntnz.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3xifegjfz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3drjfnoff.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3kxnspmrw.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3lnxvfeqh.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3zjfxogwd.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3ysrklwzd.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3sgqljsvw.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3nehjbrby.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3ldwygjzb.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3qbbacuyy.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3kcgpdoer.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3lwfviync.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3tnmpcrdv.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3elqgxxtg.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3avkpyesl.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3zkbouwgu.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3hdkblkvn.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3tncqmprb.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3xyxlqnjd.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3wxkkaebm.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3klilsbbe.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3ceqwlwlo.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3dochiizc.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3zutdeadw.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3ckpunsyt.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3zukqacpk.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3ykjtvvrn.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3aalpudeu.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3mpwkzssf.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3pqpnzqrc.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3ptyhebnh.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3mvrtqfli.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3jchveqkg.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3iczwijdf.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3ukhphexd.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3navyqjrk.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3dwttuijn.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rgxhrgsh.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3duljtkdv.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3kqzzvlfl.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3dhnfbuoo.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3ocmrzfxn.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3zjmmbwkm.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3feqhxhdi.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3hmifbamo.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3vnzshqgk.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3ejbjebnf.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zjwxikfa.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3yioloehb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3efefkzhd.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3nmmuawrn.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3bmxvizue.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3uveiczla.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3hhszrrsj.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3fqnpxjby.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3rhjoxekj.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3etbnzfre.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3jbgknsfe.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3ejczhcth.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3ajezcoia.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ghcntjyu.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3qhdjqxfu.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3whmlakiw.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3xqupkaug.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3kyxtqmto.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3dqbzwjzu.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3lkcsonva.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3ndxutijx.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3xrttxucg.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3uvjbbidl.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3whhbptcf.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3ynoqnkno.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3fdydhrmc.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3blxpeyfq.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3thkmxbrb.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3vkmajvuy.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3sheozeec.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3gmvyiyfo.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3yriugbxq.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3eacrpsgc.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3qusqlndb.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3wuwqiwrg.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3bgrzdztt.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3kgcckshg.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3scnxcmyt.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3xcrekndp.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3scafacrr.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3asizgmxj.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3slgydnic.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3nvxmhrxc.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3waskbboh.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3zzfwwdbz.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3hukvzodg.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3llvxcshl.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3yqilncvf.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3ldzgnzzu.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3cgjufdxl.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3xakrqowf.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3vzuiifzu.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3faowexwj.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3vfggmnmp.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3etxumlkh.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3bmqxzefj.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3hfbuvciv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tqkagfox.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3zzbhjtgi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rshwttvw.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jvjyzemt.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3aizhvdlc.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3irbigrml.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3cwrluluw.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3npbastpx.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3xjvrxrvk.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3emujxqbb.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3wwiesahu.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3esueqzlw.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3ppaleham.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3asndpxqy.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3psqphdih.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3ldlohdez.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3yfogeqip.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3qmjysema.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3jtndyftt.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3cfvuflku.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3oqkgfgsq.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3smshdmbv.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3buekrhgq.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3ktomgqwc.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3wsdmoufd.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3wpeoefvz.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3lkawtisk.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3uleqspdh.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3ifloeqqy.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3heuciunp.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3buldsffc.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3ejaeimfu.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3xtvmyjdu.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3cyukiuka.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3uxxyasas.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3qemenlow.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3bigisizn.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vsxggtny.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wkyvmcwk.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3yiinmsbf.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3qclochrb.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3axcdgnda.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3qvqfomcq.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3niinmofe.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3tbuizose.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3knrcjoij.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3xgtzjixa.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3nlrwfrpi.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3tzgfygmm.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3wyapimwo.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3ncspthbb.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3utovffyd.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3zgguodbb.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3aktorkjl.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3jzrkmsqn.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3zpsabgmf.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3coopivuf.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3cmjeebxs.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3sficwnfq.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3fjveexgt.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3bqbfhsqz.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3nnlhziex.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3illnozvk.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3dnwzvvkh.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3hpgpvtpa.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3klamkfwi.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3wdhpxefx.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3rkiefoox.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3unjlkhdz.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3fnwwozgk.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3exyusstm.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3januutmc.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3crhugepw.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3hzczqcci.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3rpmzsrxf.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3bzosblmo.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3bmhgzgwy.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3lfibaocm.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3dvroqpll.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3girwnrsz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jzfyfttz.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3rwllyoft.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3obgnjytd.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3llivjhef.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3ehkutucy.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3pyrjdexw.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3lzdnckqe.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3cgfejrgh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3rhpwfyfx.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3jctugryg.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3frekaxet.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3bpwlsplp.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3lpzgzjni.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3vlqiczih.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3ilniclax.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3lriwvviv.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3wjgjxwmy.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3bqegnqia.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3ufholmmx.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3gvadghpa.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3incvwjvf.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3vfnemsej.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3arviesnj.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3coywwefa.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3mjhtqxks.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3vuxmoagx.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3tujbqrlq.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3uyosmovy.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3yagxqobs.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3yjorwsxu.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3mhncsclk.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3ysyyjgfw.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3yswzvqss.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3sueexmdh.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3lndboozo.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3wzjeafhw.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3xgbgcfpv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3bkqlegwh.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3hmbmqkli.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3aktnsuhg.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3btjzmbfh.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3awldykkz.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3yzpsbztz.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3bfiiydnv.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3toajmvso.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3nyzxvems.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3zkdgkkyw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3trngrluu.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3xnrfbtvy.html


<!-- 参考信息 -->