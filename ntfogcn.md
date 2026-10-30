代发 wailian999

set -euo pipefail
来源：http://www.share.zdbjq.cn/Article/details/glnvnvlnz.sHtML

[R02] 变量赋值与使用
来源：http://blog.hesvh.cn/Article/details/gzzhephwb.sHtML

name="Tom"; echo "$name"
来源：http://wap.zdbjq.cn/Article/details/gypeuhsof.sHtML

[R03] 只读变量
来源：http://www.blog.hesvh.cn/Article/details/gedjshdgl.sHtML

readonly PI=3.14
来源：http://blog.zdbjq.cn/Article/details/ghzwwvgxi.sHtML

[R04] 位置参数
来源：http://mobile.hesvh.cn/Article/details/gzidyrnfr.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.hesvh.cn/Article/details/gjjycelgu.sHtML

[R05] 参数默认值
来源：http://baike.hesvh.cn/Article/details/gvfrcjipv.sHtML

name="${1:-default}"
来源：http://read.share.hesvh.cn/Article/details/gskqreqoc.sHtML

[R06] 判断命令是否存在
来源：http://read.share.hesvh.cn/Article/details/gwjlncdfm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.zdbjq.cn/Article/details/gwxepyrrg.sHtML

[R07] if 判断文件
来源：http://wap.hesvh.cn/Article/details/gqiqpfqbd.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.hesvh.cn/Article/details/ghanveuxm.sHtML

[R08] 数值比较
来源：http://www.blog.zdbjq.cn/Article/details/gjvyiejmc.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fehbvm.com/Article/details/grmzheycp.sHtML

[R09] 字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gffbdqyak.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.hesvh.cn/Article/details/gugixcrhy.sHtML

[R10] 正则匹配
来源：http://baike.zdbjq.cn/Article/details/gpmwlgmwr.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.hesvh.cn/Article/details/gmnmnanus.sHtML

[R11] case 多分支
来源：http://m.share.hesvh.cn/Article/details/gdpsecyht.sHtML

case "$1" in
来源：http://www.share.zdbjq.cn/Article/details/gvybluhzt.sHtML

start) echo "启动" ;;
来源：http://baike.fehbvm.com/Article/details/guiudbbku.sHtML

stop)  echo "停止" ;;
来源：http://baike.fehbvm.com/Article/details/geyyqfekp.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fehbvm.com/Article/details/gocdeusdt.sHtML

esac
来源：http://3g.hesvh.cn/Article/details/gmqiatxai.sHtML

[R12] for 遍历文件
来源：http://www.blog.fehbvm.com/Article/details/gcvvpktws.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.zdbjq.cn/Article/details/gxllhrctt.sHtML

[R13] for 计数循环
来源：http://blog.zdbjq.cn/Article/details/ghaqjdwzh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gdiqnhfqv.sHtML

[R14] C 风格 for
来源：http://blog.zdbjq.cn/Article/details/gkrcvwbaz.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/gwhgkcvul.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gojdbmbaj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.zdbjq.cn/Article/details/ghfwykewl.sHtML

[R16] until 等待条件
来源：http://baike.fehbvm.com/Article/details/gmeauaxok.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gupbqlidx.sHtML

[R17] 数组定义与取值
来源：http://www.blog.zdbjq.cn/Article/details/gvjxlxrhf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.hesvh.cn/Article/details/gwxpcmxto.sHtML

[R18] 遍历数组
来源：http://baike.hesvh.cn/Article/details/gcuccxdqh.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.hesvh.cn/Article/details/gwphwzlnm.sHtML

[R19] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/gxclsekhy.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.hesvh.cn/Article/details/gsoeyjnuq.sHtML

[R20] 关联数组（字典）
来源：http://www.share.zdbjq.cn/Article/details/gdevdcbhb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.hesvh.cn/Article/details/gdtrunouv.sHtML

[R21] 字符串长度
来源：http://baike.hesvh.cn/Article/details/gktaoovkd.sHtML

echo "${#s}"
来源：http://baike.fehbvm.com/Article/details/gzvxmuajr.sHtML

[R22] 截取子串
来源：http://www.share.fehbvm.com/Article/details/gewxivtmc.sHtML

echo "${s:0:5}"
来源：http://www.blog.fehbvm.com/Article/details/gwignldig.sHtML

[R23] 字符串替换
来源：http://wap.fehbvm.com/Article/details/gzvlucokq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.zdbjq.cn/Article/details/guqcvbtks.sHtML

[R24] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/gtanasmdo.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fehbvm.com/Article/details/gxmsjfilt.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fehbvm.com/Article/details/gqukqziyx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.hesvh.cn/Article/details/grphkkmxd.sHtML

[R26] 命令替换
来源：http://m.share.hesvh.cn/Article/details/gqxaqngtx.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fehbvm.com/Article/details/ggsqmkbft.sHtML

[R27] 算术展开
来源：http://blog.zdbjq.cn/Article/details/gknycnzfb.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.zdbjq.cn/Article/details/glxhaezzm.sHtML

[R28] 浮点运算
来源：http://www.share.zdbjq.cn/Article/details/gypgxdedz.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.hesvh.cn/Article/details/gvmdthxdf.sHtML

[R29] 定义函数
来源：http://www.share.hesvh.cn/Article/details/geqyzdukj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.zdbjq.cn/Article/details/gbdrqxrog.sHtML

[R30] 函数返回状态码
来源：http://baike.zdbjq.cn/Article/details/gvegtxang.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fehbvm.com/Article/details/gerrpbtxh.sHtML

[R31] 局部变量
来源：http://baike.fehbvm.com/Article/details/gqxderhaa.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnokusqgz.sHtML

[R32] 参数个数校验
来源：http://3g.fehbvm.com/Article/details/gbcbbkyhf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/gafhohouu.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.zdbjq.cn/Article/details/gvmpfmfdw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.zdbjq.cn/Article/details/gdanqtmii.sHtML

[R34] 退出时清理
来源：http://m.share.zdbjq.cn/Article/details/glrvfyjav.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gogdmguxa.sHtML

[R35] 后台执行并等待
来源：http://m.share.hesvh.cn/Article/details/grzvvljsd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.zdbjq.cn/Article/details/guodtgdnu.sHtML

[R36] 并发执行多个任务
来源：http://baike.hesvh.cn/Article/details/gicuiwrny.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fehbvm.com/Article/details/glgzqpzec.sHtML

[R37] 把输出赋给变量
来源：http://wap.hesvh.cn/Article/details/gwtnfdhzu.sHtML

files=$(ls -1)
来源：http://blog.zdbjq.cn/Article/details/glzznmqym.sHtML

[R38] 管道串联
来源：http://www.m.share.fehbvm.com/Article/details/gmapkqjad.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fehbvm.com/Article/details/gpyjhvkcd.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fehbvm.com/Article/details/ggqwkpwyt.sHtML

cmd > out.log 2>&1
来源：http://3g.zdbjq.cn/Article/details/grvpljbzn.sHtML

[R40] 追加写日志
来源：http://www.blog.zdbjq.cn/Article/details/gdfnipznd.sHtML

echo "log" >> out.log
来源：http://3g.zdbjq.cn/Article/details/gqwtzbutk.sHtML

[R41] 丢弃输出
来源：http://www.share.zdbjq.cn/Article/details/gipkljczv.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.zdbjq.cn/Article/details/gvycoilge.sHtML

[R42] 输入重定向
来源：http://3g.fehbvm.com/Article/details/gkjhtsvzv.sHtML

wc -l < a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gzgkpjiud.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fehbvm.com/Article/details/geqnigajm.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fehbvm.com/Article/details/gtfvlyuwd.sHtML

[R44] 按修改时间查找
来源：http://blog.hesvh.cn/Article/details/giytrzjwb.sHtML

find . -mtime -7 -type f
来源：http://www.share.zdbjq.cn/Article/details/gjjbastzd.sHtML

[R45] 批量删除
来源：http://wap.fehbvm.com/Article/details/gifhfroqu.sHtML

find . -name "*.tmp" -delete
来源：http://3g.zdbjq.cn/Article/details/gmsnjescz.sHtML

[R46] 递归替换文件内容
来源：http://baike.fehbvm.com/Article/details/gzoiwypef.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.hesvh.cn/Article/details/gpmssyzca.sHtML

[R47] sed 单行替换
来源：http://m.share.fehbvm.com/Article/details/gemraillx.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gxmcpmqlm.sHtML

[R48] awk 取指定列
来源：http://blog.zdbjq.cn/Article/details/gpdcdppek.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.hesvh.cn/Article/details/gkknmjdfa.sHtML

[R49] awk 带条件
来源：http://read.share.hesvh.cn/Article/details/gxiltftvk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.hesvh.cn/Article/details/gsnqwqoyc.sHtML

[R50] awk 求和
来源：http://www.share.hesvh.cn/Article/details/gpiscucwe.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.hesvh.cn/Article/details/grygxbmex.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fehbvm.com/Article/details/gvswtlgby.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.zdbjq.cn/Article/details/gunorxjuo.sHtML

[R52] 统计行数
来源：http://www.blog.hesvh.cn/Article/details/ghoazxxio.sHtML

wc -l a.txt
来源：http://mobile.fehbvm.com/Article/details/gatgwtorh.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.zdbjq.cn/Article/details/gzvgztbye.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.zdbjq.cn/Article/details/gmqlieasw.sHtML

[R54] 比较两个文件
来源：http://m.share.hesvh.cn/Article/details/gaaohxwwt.sHtML

diff a.txt b.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gpvaqachw.sHtML

[R55] 压缩与解压
来源：http://3g.zdbjq.cn/Article/details/gjwwttfio.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.zdbjq.cn/Article/details/gtuislord.sHtML

[R56] 远程拷贝
来源：http://3g.hesvh.cn/Article/details/gridrcrik.sHtML

scp file user@host:/path/
来源：http://www.blog.zdbjq.cn/Article/details/gcsbirzlx.sHtML

[R57] 远程执行命令
来源：http://mobile.zdbjq.cn/Article/details/gmzummqly.sHtML

ssh user@host 'uptime'
来源：http://wap.hesvh.cn/Article/details/goezagfqm.sHtML

[R58] 下载文件
来源：http://baike.fehbvm.com/Article/details/ggobwdbjm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.zdbjq.cn/Article/details/gjtjjebjp.sHtML

[R59] 发 POST JSON
来源：http://blog.fehbvm.com/Article/details/gbstwphpt.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fehbvm.com/Article/details/gvjnaxbrl.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/gwqrbjyeh.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.zdbjq.cn/Article/details/gldoqzgbf.sHtML

[R61] 磁盘占用
来源：http://www.m.share.zdbjq.cn/Article/details/gqktcllpk.sHtML

df -h;  du -sh *
来源：http://read.share.hesvh.cn/Article/details/glbjtrsvq.sHtML

[R62] 找最占空间的文件
来源：http://blog.hesvh.cn/Article/details/gcebrwfqw.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.hesvh.cn/Article/details/gzoujvrkz.sHtML

[R63] 内存与进程
来源：http://m.share.zdbjq.cn/Article/details/gqieajlhg.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fehbvm.com/Article/details/grwflajgu.sHtML

[R64] 结束进程
来源：http://mobile.hesvh.cn/Article/details/gscrjqhqs.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.hesvh.cn/Article/details/giwcawjlu.sHtML

[R65] 查看端口占用
来源：http://www.m.share.zdbjq.cn/Article/details/gkbbbeemo.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fehbvm.com/Article/details/gvrjmcrsp.sHtML

[R66] 定时任务
来源：http://m.share.hesvh.cn/Article/details/gaaorfwfx.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.hesvh.cn/Article/details/gyryrdqyy.sHtML

[R67] 生成随机十六进制串
来源：http://wap.zdbjq.cn/Article/details/gmkhcrnrv.sHtML

openssl rand -hex 16
来源：http://www.share.fehbvm.com/Article/details/grfytlvur.sHtML

[R68] 计算文件校验值
来源：http://read.share.hesvh.cn/Article/details/gywywujoq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fehbvm.com/Article/details/gkqzkwumv.sHtML

[R69] 生成随机密码
来源：http://www.m.share.hesvh.cn/Article/details/gfajhcjyt.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.hesvh.cn/Article/details/gthmvdojj.sHtML

[R70] 时间戳与互转
来源：http://wap.zdbjq.cn/Article/details/gcofgwwet.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.zdbjq.cn/Article/details/gpgslyzdm.sHtML

[R71] 日期格式化
来源：http://blog.hesvh.cn/Article/details/gqccxzabl.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.zdbjq.cn/Article/details/gkybdjyfu.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fehbvm.com/Article/details/gxaufgyum.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/gvdbxszdw.sHtML

[R73] 分割大日志
来源：http://wap.fehbvm.com/Article/details/gqyikdomi.sHtML

split -l 1000 big.log part_
来源：http://wap.zdbjq.cn/Article/details/gimvryxuc.sHtML

[R74] 批量重命名
来源：http://baike.fehbvm.com/Article/details/gqhkingjn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.hesvh.cn/Article/details/gwykkflpd.sHtML

[R75] 导出环境变量
来源：http://www.share.fehbvm.com/Article/details/gljfhufnq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fehbvm.com/Article/details/gkieumrrk.sHtML

[R76] 使用临时文件
来源：http://m.share.hesvh.cn/Article/details/gdiwoewtj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.zdbjq.cn/Article/details/gpczsnrls.sHtML

[R77] 读取用户输入
来源：http://baike.zdbjq.cn/Article/details/gfrnnflck.sHtML

read -rp "请输入: " ans
来源：http://blog.zdbjq.cn/Article/details/giwalttjb.sHtML

[R78] 交互式菜单
来源：http://www.share.hesvh.cn/Article/details/grujkvvvo.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fehbvm.com/Article/details/gmgabtrna.sHtML

[R79] 解析命令行选项
来源：http://blog.fehbvm.com/Article/details/gvtkmjbvt.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.hesvh.cn/Article/details/gnxuphggr.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.hesvh.cn/Article/details/grbapqlvj.sHtML

time ./run.sh
来源：http://wap.fehbvm.com/Article/details/glxrspmqz.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gravwdpjq.sHtML

S. C / C++ 专题
来源：http://3g.fehbvm.com/Article/details/gijqnxgyy.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gulsuvfbo.sHtML

[S01] C：Hello World
来源：http://mobile.hesvh.cn/Article/details/guenssjys.sHtML

#include <stdio.h>
来源：http://www.blog.fehbvm.com/Article/details/gyzdhxvek.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.zdbjq.cn/Article/details/gtesqcjhp.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fehbvm.com/Article/details/gqeowtjph.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.zdbjq.cn/Article/details/gcybofshs.sHtML

[S03] C：读入整数
来源：http://wap.hesvh.cn/Article/details/gpdyehbnf.sHtML

int x; scanf("%d", &x);
来源：http://wap.fehbvm.com/Article/details/gzbxorwxd.sHtML

[S04] C：字符串复制
来源：http://www.share.hesvh.cn/Article/details/gfmhmmarl.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fehbvm.com/Article/details/gymarmaqq.sHtML

[S05] C：字符串长度
来源：http://mobile.zdbjq.cn/Article/details/gzmhpusix.sHtML

strlen(s)
来源：http://www.share.fehbvm.com/Article/details/gaokdqsqn.sHtML

[S06] C：字符串比较
来源：http://mobile.hesvh.cn/Article/details/gzxmpjyqn.sHtML

strcmp(a, b) == 0
来源：http://read.share.fehbvm.com/Article/details/gormcbwey.sHtML

[S07] C：数组遍历求和
来源：http://read.share.zdbjq.cn/Article/details/gvcmdwrei.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fehbvm.com/Article/details/guecbhupw.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.zdbjq.cn/Article/details/gixrtvndr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.zdbjq.cn/Article/details/gwclocpbr.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.zdbjq.cn/Article/details/gmkzlhlov.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fehbvm.com/Article/details/gpgfxhcvk.sHtML

[S10] C：指针与解引用
来源：http://blog.hesvh.cn/Article/details/gvppabght.sHtML

int *p = &a;  *p = 5;
来源：http://3g.zdbjq.cn/Article/details/gewrfjzms.sHtML

[S11] C：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gaspmjshn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.zdbjq.cn/Article/details/giwquavem.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.zdbjq.cn/Article/details/glwimbqhr.sHtML

fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/gdassherg.sHtML

[S12] C：写文件
来源：http://3g.fehbvm.com/Article/details/gpubruxoz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gdcdlbmnb.sHtML

[S13] C：宏定义
来源：http://mobile.fehbvm.com/Article/details/guttazlmq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.hesvh.cn/Article/details/gurtchlab.sHtML

[S14] C：枚举
来源：http://www.blog.fehbvm.com/Article/details/giwmflgsa.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fehbvm.com/Article/details/ggvvnrwnb.sHtML

[S15] C：类型转换
来源：http://blog.hesvh.cn/Article/details/gmbxtcivi.sHtML

(double) a / b
来源：http://blog.zdbjq.cn/Article/details/gwskclrke.sHtML

[S16] C：位操作置位
来源：http://3g.zdbjq.cn/Article/details/geukxprjs.sHtML

x |= (1 << 3);
来源：http://www.blog.fehbvm.com/Article/details/gvhndmdih.sHtML

[S17] C：安全拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gfbrrigpt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.zdbjq.cn/Article/details/gfdpjkils.sHtML

[S18] C：命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/gboxxmyid.sHtML

int main(int argc, char **argv)
来源：http://m.share.fehbvm.com/Article/details/gmyczbfuv.sHtML

[S19] C：快速排序
来源：http://blog.fehbvm.com/Article/details/gvmlkhqod.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/glrnxlnvp.sHtML

[S20] C：二分查找
来源：http://blog.fehbvm.com/Article/details/guroxixru.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/gkzfeucau.sHtML

[S21] C：字符类别判断
来源：http://mobile.fehbvm.com/Article/details/grrhwdvib.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.zdbjq.cn/Article/details/gjvycykap.sHtML

[S22] C：字符串转数字
来源：http://read.share.hesvh.cn/Article/details/gtrhpmdje.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fehbvm.com/Article/details/gsucwvtgo.sHtML

[S23] C：随机数
来源：http://m.share.fehbvm.com/Article/details/gmgljtbfo.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.zdbjq.cn/Article/details/gvpoqvnlu.sHtML

[S24] C：获取本地时间
来源：http://baike.zdbjq.cn/Article/details/gdpffiemh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fehbvm.com/Article/details/geqxfgefo.sHtML

[S25] C：内存拷贝
来源：http://blog.hesvh.cn/Article/details/gaxymuwxu.sHtML

memcpy(dst, src, n);
来源：http://baike.zdbjq.cn/Article/details/gxxclnuys.sHtML

[S26] C：内存清零
来源：http://www.share.zdbjq.cn/Article/details/gvyjjuqpo.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fehbvm.com/Article/details/gwtgqbzwk.sHtML

[S27] C：定义常量
来源：http://baike.fehbvm.com/Article/details/gencmmqcx.sHtML

const double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gcmbyljbj.sHtML

[S28] C：静态变量
来源：http://3g.zdbjq.cn/Article/details/gcwroffbu.sHtML

static int counter = 0;
来源：http://3g.fehbvm.com/Article/details/gyvvnbbao.sHtML

[S29] C：变参函数
来源：http://www.m.share.zdbjq.cn/Article/details/gidhubavv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.hesvh.cn/Article/details/gqgswtgqt.sHtML

[S30] C：头文件保护
来源：http://www.blog.fehbvm.com/Article/details/gwtbjgmcc.sHtML

#ifndef X_H
来源：http://mobile.hesvh.cn/Article/details/gakwmjqtx.sHtML

#define X_H
来源：http://baike.fehbvm.com/Article/details/gmmlkwhvw.sHtML

#endif
来源：http://baike.zdbjq.cn/Article/details/gsofpncud.sHtML

[S31] C++：Hello World
来源：http://www.share.zdbjq.cn/Article/details/ghaddokkp.sHtML

#include <iostream>
来源：http://read.share.fehbvm.com/Article/details/gfkqojpvk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.hesvh.cn/Article/details/gmpliyvjh.sHtML

[S32] C++：字符串
来源：http://read.share.zdbjq.cn/Article/details/gfrabhtyn.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.hesvh.cn/Article/details/gzhuwrrnx.sHtML

[S33] C++：vector 增删
来源：http://baike.hesvh.cn/Article/details/gggrqymla.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fehbvm.com/Article/details/gvlfsmbth.sHtML

[S34] C++：遍历 vector
来源：http://baike.zdbjq.cn/Article/details/gvbaphjvg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fehbvm.com/Article/details/georspgrg.sHtML

[S35] C++：map
来源：http://www.blog.zdbjq.cn/Article/details/glcelkytq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gaaumbekl.sHtML

[S36] C++：unordered_map
来源：http://mobile.hesvh.cn/Article/details/gowlomwjl.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gltygfbui.sHtML

[S37] C++：set
来源：http://www.share.hesvh.cn/Article/details/ghvdyfxgm.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.zdbjq.cn/Article/details/gkhotrwgi.sHtML

[S38] C++：排序
来源：http://mobile.fehbvm.com/Article/details/ggopaeulr.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fehbvm.com/Article/details/gxihvayzk.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.zdbjq.cn/Article/details/glblobumy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.zdbjq.cn/Article/details/gwmrgjdgc.sHtML

[S40] C++：查找元素
来源：http://blog.zdbjq.cn/Article/details/glrekgyen.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.zdbjq.cn/Article/details/gsmnojihd.sHtML

[S41] C++：类与构造函数
来源：http://blog.fehbvm.com/Article/details/gejwwodsr.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fehbvm.com/Article/details/gffuwshsl.sHtML

[S42] C++：继承与虚函数
来源：http://wap.hesvh.cn/Article/details/gyddtretf.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.zdbjq.cn/Article/details/gqyjnwtlj.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fehbvm.com/Article/details/gcpdakywd.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.zdbjq.cn/Article/details/gvwirsydj.sHtML

[S44] C++：引用传参
来源：http://m.share.hesvh.cn/Article/details/gmrcsjmhp.sHtML

void inc(int &x) { ++x; }
来源：http://3g.hesvh.cn/Article/details/gnctmovsd.sHtML

[S45] C++：lambda
来源：http://www.share.fehbvm.com/Article/details/gahypijgr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.zdbjq.cn/Article/details/gbddffyqc.sHtML

[S46] C++：函数模板
来源：http://baike.fehbvm.com/Article/details/gbmngktgn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.hesvh.cn/Article/details/gbteelsdb.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.zdbjq.cn/Article/details/ghsqyjgot.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fehbvm.com/Article/details/gruswmqhj.sHtML

[S48] C++：逐行读文件
来源：http://3g.hesvh.cn/Article/details/ghrnzbadj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.zdbjq.cn/Article/details/gxjhudatj.sHtML

while (std::getline(in, line)) { }
来源：http://3g.zdbjq.cn/Article/details/gnoacwsdl.sHtML

[S49] C++：写文件
来源：http://www.share.fehbvm.com/Article/details/gakdzxjvw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.zdbjq.cn/Article/details/gvwttgaov.sHtML

[S50] C++：格式化数字
来源：http://m.share.fehbvm.com/Article/details/gskgihawe.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gwdabhqxs.sHtML

[S51] C++：显式类型转换
来源：http://m.share.zdbjq.cn/Article/details/gdezejdfg.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.hesvh.cn/Article/details/gqdmbqsmg.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.hesvh.cn/Article/details/gmwdorjew.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.zdbjq.cn/Article/details/giyromahc.sHtML

[S53] C++：移动语义
来源：http://blog.hesvh.cn/Article/details/gffamkpve.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.zdbjq.cn/Article/details/gntxeocrw.sHtML

[S54] C++：异常处理
来源：http://read.share.fehbvm.com/Article/details/gafkogmwt.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.zdbjq.cn/Article/details/garrhdqib.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fehbvm.com/Article/details/gwnniugkk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fehbvm.com/Article/details/gsbwrobgy.sHtML

[S56] C++：optional
来源：http://baike.zdbjq.cn/Article/details/gyatggrdx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.zdbjq.cn/Article/details/gckablgsc.sHtML

[S57] C++：编译期常量
来源：http://read.share.fehbvm.com/Article/details/gmhdehnbb.sHtML

constexpr int N = 10;
来源：http://wap.fehbvm.com/Article/details/ghvzjiues.sHtML

[S58] C++：命名空间
来源：http://www.blog.zdbjq.cn/Article/details/gevctisnm.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.hesvh.cn/Article/details/gifojsyzt.sHtML

[S59] C++：静态断言
来源：http://www.share.fehbvm.com/Article/details/gqrfkslwf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.zdbjq.cn/Article/details/glyjczbiq.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.hesvh.cn/Article/details/gafvukagd.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fehbvm.com/Article/details/gygsxtomx.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gtnfmxkqs.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.zdbjq.cn/Article/details/geqmlqfbj.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gceemizqp.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fehbvm.com/Article/details/gvrcfhavm.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/gfgjnadrs.sHtML

[T02] Kotlin：变量
来源：http://m.share.hesvh.cn/Article/details/gdddzkoxh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fehbvm.com/Article/details/grkabykdv.sHtML


<!-- 参考信息 -->