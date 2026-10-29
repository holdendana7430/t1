代发 wailian999

set -euo pipefail
来源：http://m.share.fehbvm.com/Article/details/gtahvduie.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fehbvm.com/Article/details/gidxqxsin.sHtML

name="Tom"; echo "$name"
来源：http://3g.fehbvm.com/Article/details/giciqllxy.sHtML

[R03] 只读变量
来源：http://3g.hesvh.cn/Article/details/gncrnlgfs.sHtML

readonly PI=3.14
来源：http://wap.zdbjq.cn/Article/details/garyzewac.sHtML

[R04] 位置参数
来源：http://mobile.fehbvm.com/Article/details/gmtgwjxzq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.zdbjq.cn/Article/details/giafehkuc.sHtML

[R05] 参数默认值
来源：http://wap.hesvh.cn/Article/details/gyqwtdsfd.sHtML

name="${1:-default}"
来源：http://read.share.hesvh.cn/Article/details/gsmczpgiv.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fehbvm.com/Article/details/guqehxtqd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gwzgxrhhv.sHtML

[R07] if 判断文件
来源：http://wap.zdbjq.cn/Article/details/gnjmfiotm.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.hesvh.cn/Article/details/gcvdpkllt.sHtML

[R08] 数值比较
来源：http://read.share.zdbjq.cn/Article/details/gmlozbxzi.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fehbvm.com/Article/details/gqfemolun.sHtML

[R09] 字符串比较
来源：http://mobile.hesvh.cn/Article/details/guklvumfy.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/ggldtdyws.sHtML

[R10] 正则匹配
来源：http://www.share.hesvh.cn/Article/details/guxxarhta.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gsajtaedx.sHtML

[R11] case 多分支
来源：http://baike.hesvh.cn/Article/details/guhdxubbz.sHtML

case "$1" in
来源：http://www.share.fehbvm.com/Article/details/gcbdyokqx.sHtML

start) echo "启动" ;;
来源：http://www.blog.hesvh.cn/Article/details/gumihpxfo.sHtML

stop)  echo "停止" ;;
来源：http://m.share.zdbjq.cn/Article/details/gzprxaaye.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.hesvh.cn/Article/details/gojnlstiu.sHtML

esac
来源：http://mobile.hesvh.cn/Article/details/gwjmmerbc.sHtML

[R12] for 遍历文件
来源：http://blog.zdbjq.cn/Article/details/gqfqaobum.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.hesvh.cn/Article/details/ghxdbgqyv.sHtML

[R13] for 计数循环
来源：http://3g.zdbjq.cn/Article/details/guyaovhkj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/gwevyumol.sHtML

[R14] C 风格 for
来源：http://baike.hesvh.cn/Article/details/gmlemwnhd.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gppidsoeq.sHtML

[R15] while 逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gdypmuzhg.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.hesvh.cn/Article/details/gpdhgiphw.sHtML

[R16] until 等待条件
来源：http://3g.fehbvm.com/Article/details/gqwbqjjks.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/gkkgyapbp.sHtML

[R17] 数组定义与取值
来源：http://3g.hesvh.cn/Article/details/gxrlopqpl.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.hesvh.cn/Article/details/gyhbqaxog.sHtML

[R18] 遍历数组
来源：http://www.share.fehbvm.com/Article/details/gbedwbjcs.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fehbvm.com/Article/details/gkxkjewgo.sHtML

[R19] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/gollhrabx.sHtML

echo "${#arr[@]}"
来源：http://3g.zdbjq.cn/Article/details/gfcdmxzny.sHtML

[R20] 关联数组（字典）
来源：http://3g.fehbvm.com/Article/details/gariiknrx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.hesvh.cn/Article/details/gsiorweqa.sHtML

[R21] 字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/ghwqflfqe.sHtML

echo "${#s}"
来源：http://www.share.zdbjq.cn/Article/details/gtgefgeqz.sHtML

[R22] 截取子串
来源：http://3g.zdbjq.cn/Article/details/gxvrynvjk.sHtML

echo "${s:0:5}"
来源：http://blog.hesvh.cn/Article/details/gwjtzzpcg.sHtML

[R23] 字符串替换
来源：http://read.share.fehbvm.com/Article/details/gzkexaykv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.zdbjq.cn/Article/details/gmfheyisw.sHtML

[R24] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/gnmxertwa.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.zdbjq.cn/Article/details/guuodwjfu.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.zdbjq.cn/Article/details/gyxnwkpqo.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.zdbjq.cn/Article/details/ggcgxovds.sHtML

[R26] 命令替换
来源：http://read.share.zdbjq.cn/Article/details/geknfgoof.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.zdbjq.cn/Article/details/gmkutlbay.sHtML

[R27] 算术展开
来源：http://www.m.share.zdbjq.cn/Article/details/gjqqtpwqv.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fehbvm.com/Article/details/gjknrfsth.sHtML

[R28] 浮点运算
来源：http://mobile.zdbjq.cn/Article/details/grvfroeql.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.zdbjq.cn/Article/details/gooepdenm.sHtML

[R29] 定义函数
来源：http://www.share.hesvh.cn/Article/details/gbywlgcxg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fehbvm.com/Article/details/gwgltbhzu.sHtML

[R30] 函数返回状态码
来源：http://baike.hesvh.cn/Article/details/grsfwdpli.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.zdbjq.cn/Article/details/gksoexazw.sHtML

[R31] 局部变量
来源：http://wap.fehbvm.com/Article/details/ghsvefskw.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fehbvm.com/Article/details/glgumhcwy.sHtML

[R32] 参数个数校验
来源：http://wap.hesvh.cn/Article/details/gachzkzkg.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/gopkdnhmd.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.hesvh.cn/Article/details/gvansuqmk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.zdbjq.cn/Article/details/guuqpctwo.sHtML

[R34] 退出时清理
来源：http://m.share.zdbjq.cn/Article/details/gitikviez.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/ghruenyht.sHtML

[R35] 后台执行并等待
来源：http://3g.hesvh.cn/Article/details/geillatih.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.hesvh.cn/Article/details/gjsmgsqny.sHtML

[R36] 并发执行多个任务
来源：http://mobile.zdbjq.cn/Article/details/gsleupfua.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.zdbjq.cn/Article/details/gxbplfwdn.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fehbvm.com/Article/details/gqlqmqgxi.sHtML

files=$(ls -1)
来源：http://m.share.zdbjq.cn/Article/details/gghgklsbt.sHtML

[R38] 管道串联
来源：http://read.share.hesvh.cn/Article/details/gadurydlb.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.zdbjq.cn/Article/details/glhoysqeu.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.zdbjq.cn/Article/details/gohcrkwpb.sHtML

cmd > out.log 2>&1
来源：http://baike.hesvh.cn/Article/details/gqtclblqv.sHtML

[R40] 追加写日志
来源：http://wap.zdbjq.cn/Article/details/gunfekgcv.sHtML

echo "log" >> out.log
来源：http://mobile.fehbvm.com/Article/details/ggkgierzd.sHtML

[R41] 丢弃输出
来源：http://www.blog.zdbjq.cn/Article/details/gmqqmydvw.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fehbvm.com/Article/details/glwjvlxyc.sHtML

[R42] 输入重定向
来源：http://m.share.fehbvm.com/Article/details/gzgnmlkqf.sHtML

wc -l < a.txt
来源：http://3g.hesvh.cn/Article/details/gqyfegebw.sHtML

[R43] 按名字查找文件
来源：http://m.share.zdbjq.cn/Article/details/gojxvhpzc.sHtML

find . -name "*.log" -type f
来源：http://3g.hesvh.cn/Article/details/gljogadwb.sHtML

[R44] 按修改时间查找
来源：http://m.share.hesvh.cn/Article/details/gsbjsdlvw.sHtML

find . -mtime -7 -type f
来源：http://m.share.zdbjq.cn/Article/details/ghvfltraz.sHtML

[R45] 批量删除
来源：http://read.share.fehbvm.com/Article/details/gpsqcjstu.sHtML

find . -name "*.tmp" -delete
来源：http://blog.zdbjq.cn/Article/details/gywxagkve.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.zdbjq.cn/Article/details/gfoayjdez.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.hesvh.cn/Article/details/gjunzrawg.sHtML

[R47] sed 单行替换
来源：http://www.blog.fehbvm.com/Article/details/gundqdmkl.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.hesvh.cn/Article/details/guguvdqah.sHtML

[R48] awk 取指定列
来源：http://mobile.hesvh.cn/Article/details/gmyisodru.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gisxdbkvr.sHtML

[R49] awk 带条件
来源：http://www.m.share.zdbjq.cn/Article/details/gzddeavad.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fehbvm.com/Article/details/ghlukaxno.sHtML

[R50] awk 求和
来源：http://read.share.zdbjq.cn/Article/details/gwnmsuyov.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fehbvm.com/Article/details/grxaexvap.sHtML

[R51] 排序去重取前几
来源：http://blog.zdbjq.cn/Article/details/geaijchfn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fehbvm.com/Article/details/ggnnhhcxv.sHtML

[R52] 统计行数
来源：http://read.share.hesvh.cn/Article/details/gvevanvmd.sHtML

wc -l a.txt
来源：http://read.share.hesvh.cn/Article/details/gfqkxmhab.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fehbvm.com/Article/details/gjmcqiwik.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.zdbjq.cn/Article/details/gkpruscvf.sHtML

[R54] 比较两个文件
来源：http://read.share.hesvh.cn/Article/details/ghpvqdpay.sHtML

diff a.txt b.txt
来源：http://baike.hesvh.cn/Article/details/gcaopzbho.sHtML

[R55] 压缩与解压
来源：http://www.share.fehbvm.com/Article/details/grdrvodbw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.hesvh.cn/Article/details/gjmscqgbf.sHtML

[R56] 远程拷贝
来源：http://baike.zdbjq.cn/Article/details/gfzmmvoci.sHtML

scp file user@host:/path/
来源：http://read.share.zdbjq.cn/Article/details/gwccgcxkc.sHtML

[R57] 远程执行命令
来源：http://www.share.zdbjq.cn/Article/details/gbtbiosim.sHtML

ssh user@host 'uptime'
来源：http://baike.hesvh.cn/Article/details/gmsalrpgx.sHtML

[R58] 下载文件
来源：http://blog.zdbjq.cn/Article/details/glkybsdcg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.zdbjq.cn/Article/details/gbhfxokxj.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fehbvm.com/Article/details/gsvmrsplc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.hesvh.cn/Article/details/gpwvlvqri.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/gwflryxma.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fehbvm.com/Article/details/gnzemlfzw.sHtML

[R61] 磁盘占用
来源：http://www.share.hesvh.cn/Article/details/gwctkdbfb.sHtML

df -h;  du -sh *
来源：http://read.share.fehbvm.com/Article/details/grpaxnnos.sHtML

[R62] 找最占空间的文件
来源：http://3g.hesvh.cn/Article/details/grrzlyyfp.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.hesvh.cn/Article/details/gqffmozdw.sHtML

[R63] 内存与进程
来源：http://wap.fehbvm.com/Article/details/gtucyidoe.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fehbvm.com/Article/details/grhzeroft.sHtML

[R64] 结束进程
来源：http://www.blog.hesvh.cn/Article/details/gkyvmdewm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.hesvh.cn/Article/details/garofdwjc.sHtML

[R65] 查看端口占用
来源：http://read.share.fehbvm.com/Article/details/gapzwubzn.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fehbvm.com/Article/details/gdqlvnwap.sHtML

[R66] 定时任务
来源：http://mobile.fehbvm.com/Article/details/giijoioya.sHtML

crontab -e;  crontab -l
来源：http://www.share.fehbvm.com/Article/details/gpyldunbu.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.zdbjq.cn/Article/details/gozirarlx.sHtML

openssl rand -hex 16
来源：http://3g.hesvh.cn/Article/details/gmsghtyam.sHtML

[R68] 计算文件校验值
来源：http://m.share.hesvh.cn/Article/details/gyyiqpvav.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fehbvm.com/Article/details/gksjsihgx.sHtML

[R69] 生成随机密码
来源：http://3g.zdbjq.cn/Article/details/gfowrvqts.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.hesvh.cn/Article/details/gcrvrqxbb.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.hesvh.cn/Article/details/guxoescct.sHtML

date +%s;  date -d @1700000000
来源：http://blog.zdbjq.cn/Article/details/guaorzyid.sHtML

[R71] 日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gnvcdsrtw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.zdbjq.cn/Article/details/ghgkqorpo.sHtML

[R72] 等待端口就绪
来源：http://www.share.zdbjq.cn/Article/details/gscsieivm.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/gxysbpiko.sHtML

[R73] 分割大日志
来源：http://baike.zdbjq.cn/Article/details/gfyvnchmm.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.zdbjq.cn/Article/details/ggobfjgat.sHtML

[R74] 批量重命名
来源：http://www.blog.zdbjq.cn/Article/details/gofcpepfz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.hesvh.cn/Article/details/glybielyl.sHtML

[R75] 导出环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gacrpetvf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.hesvh.cn/Article/details/gbfstinps.sHtML

[R76] 使用临时文件
来源：http://wap.fehbvm.com/Article/details/geqkkfaoi.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/gmnhohneo.sHtML

[R77] 读取用户输入
来源：http://read.share.hesvh.cn/Article/details/ggiylixlr.sHtML

read -rp "请输入: " ans
来源：http://mobile.zdbjq.cn/Article/details/gcoralvgp.sHtML

[R78] 交互式菜单
来源：http://m.share.zdbjq.cn/Article/details/gusypkujf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fehbvm.com/Article/details/gzqbjiuvj.sHtML

[R79] 解析命令行选项
来源：http://wap.hesvh.cn/Article/details/gfyuwpsys.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.hesvh.cn/Article/details/gxggizevv.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.zdbjq.cn/Article/details/gxqtivfvo.sHtML

time ./run.sh
来源：http://wap.fehbvm.com/Article/details/gdaeihwxx.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ggdmgksjg.sHtML

S. C / C++ 专题
来源：http://wap.fehbvm.com/Article/details/guzkrlnih.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gahnupzhv.sHtML

[S01] C：Hello World
来源：http://wap.hesvh.cn/Article/details/goudoohnj.sHtML

#include <stdio.h>
来源：http://www.share.zdbjq.cn/Article/details/gvfgfwwfo.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.hesvh.cn/Article/details/ghqwmuece.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fehbvm.com/Article/details/gdcbzzfvd.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.zdbjq.cn/Article/details/gmmnvqelh.sHtML

[S03] C：读入整数
来源：http://3g.zdbjq.cn/Article/details/gyzuknhvg.sHtML

int x; scanf("%d", &x);
来源：http://3g.fehbvm.com/Article/details/gtudibavl.sHtML

[S04] C：字符串复制
来源：http://3g.zdbjq.cn/Article/details/gforjhinm.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fehbvm.com/Article/details/gbwezymgl.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/gybbvjywm.sHtML

strlen(s)
来源：http://read.share.fehbvm.com/Article/details/gfzfpmbcu.sHtML

[S06] C：字符串比较
来源：http://baike.hesvh.cn/Article/details/ghaicedus.sHtML

strcmp(a, b) == 0
来源：http://baike.hesvh.cn/Article/details/gghtyhetp.sHtML

[S07] C：数组遍历求和
来源：http://wap.zdbjq.cn/Article/details/geuoclfzp.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fehbvm.com/Article/details/glubnyxhf.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fehbvm.com/Article/details/gpuptervc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fehbvm.com/Article/details/gfcmnnkxc.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fehbvm.com/Article/details/gevmostsq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fehbvm.com/Article/details/gkpeolxbx.sHtML

[S10] C：指针与解引用
来源：http://www.share.fehbvm.com/Article/details/gdrhprhxl.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fehbvm.com/Article/details/gkeckugve.sHtML

[S11] C：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gnsvpfitt.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fehbvm.com/Article/details/gjwwvjfef.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.hesvh.cn/Article/details/guoisfqrz.sHtML

fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/gnddkjrho.sHtML

[S12] C：写文件
来源：http://m.share.hesvh.cn/Article/details/gdwinrfjw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gimvvropy.sHtML

[S13] C：宏定义
来源：http://mobile.zdbjq.cn/Article/details/ggmrowwua.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.zdbjq.cn/Article/details/ggewlixso.sHtML

[S14] C：枚举
来源：http://baike.zdbjq.cn/Article/details/gusqfwleb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.zdbjq.cn/Article/details/gqgfsvaoi.sHtML

[S15] C：类型转换
来源：http://wap.fehbvm.com/Article/details/gkzvprmay.sHtML

(double) a / b
来源：http://3g.zdbjq.cn/Article/details/ghowmgxgn.sHtML

[S16] C：位操作置位
来源：http://baike.fehbvm.com/Article/details/gywywjvcz.sHtML

x |= (1 << 3);
来源：http://www.m.share.fehbvm.com/Article/details/gksgcgoff.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gzsxreroo.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.hesvh.cn/Article/details/gojxyytqt.sHtML

[S18] C：命令行参数
来源：http://read.share.zdbjq.cn/Article/details/gnbrsuejy.sHtML

int main(int argc, char **argv)
来源：http://read.share.hesvh.cn/Article/details/ghxfamafw.sHtML

[S19] C：快速排序
来源：http://read.share.zdbjq.cn/Article/details/ggjgvektb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/gtigltnjg.sHtML

[S20] C：二分查找
来源：http://www.blog.zdbjq.cn/Article/details/gqujbfjok.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/gnlceweyi.sHtML

[S21] C：字符类别判断
来源：http://wap.hesvh.cn/Article/details/galhjfqwh.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fehbvm.com/Article/details/gsmxegsfd.sHtML

[S22] C：字符串转数字
来源：http://wap.zdbjq.cn/Article/details/gykrptvqj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.zdbjq.cn/Article/details/gfdyvyitm.sHtML

[S23] C：随机数
来源：http://www.blog.zdbjq.cn/Article/details/gjkdtercq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fehbvm.com/Article/details/gdikqkwek.sHtML

[S24] C：获取本地时间
来源：http://blog.fehbvm.com/Article/details/gwhdbhqab.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fehbvm.com/Article/details/gecrtmsmi.sHtML

[S25] C：内存拷贝
来源：http://m.share.fehbvm.com/Article/details/gbxupsswn.sHtML

memcpy(dst, src, n);
来源：http://read.share.hesvh.cn/Article/details/gvhnqltpn.sHtML

[S26] C：内存清零
来源：http://read.share.fehbvm.com/Article/details/gehsyhqtk.sHtML

memset(a, 0, sizeof a);
来源：http://wap.hesvh.cn/Article/details/gvjuwnenr.sHtML

[S27] C：定义常量
来源：http://www.blog.hesvh.cn/Article/details/gfifbkfjw.sHtML

const double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gfnxuxdgg.sHtML

[S28] C：静态变量
来源：http://read.share.fehbvm.com/Article/details/gvhrtkvrv.sHtML

static int counter = 0;
来源：http://3g.fehbvm.com/Article/details/grsvnembe.sHtML

[S29] C：变参函数
来源：http://wap.zdbjq.cn/Article/details/gneyvckml.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fehbvm.com/Article/details/guuywnoei.sHtML

[S30] C：头文件保护
来源：http://3g.zdbjq.cn/Article/details/gooirbmrl.sHtML

#ifndef X_H
来源：http://www.m.share.hesvh.cn/Article/details/gobpkajcr.sHtML

#define X_H
来源：http://m.share.zdbjq.cn/Article/details/gsoobpivp.sHtML

#endif
来源：http://wap.zdbjq.cn/Article/details/gimmkcusy.sHtML

[S31] C++：Hello World
来源：http://wap.fehbvm.com/Article/details/gxqxnabyr.sHtML

#include <iostream>
来源：http://baike.zdbjq.cn/Article/details/gqdkealbg.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.zdbjq.cn/Article/details/gvtufuwkw.sHtML

[S32] C++：字符串
来源：http://mobile.hesvh.cn/Article/details/gfghomgdf.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fehbvm.com/Article/details/gcgiknfkq.sHtML

[S33] C++：vector 增删
来源：http://m.share.hesvh.cn/Article/details/gesdcmluq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.zdbjq.cn/Article/details/gfneyftjv.sHtML

[S34] C++：遍历 vector
来源：http://mobile.zdbjq.cn/Article/details/goufuzoow.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.hesvh.cn/Article/details/gryadjgda.sHtML

[S35] C++：map
来源：http://wap.fehbvm.com/Article/details/glibrnasj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gegwhxhmb.sHtML

[S36] C++：unordered_map
来源：http://m.share.fehbvm.com/Article/details/grlkygbif.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/gpbwkpckc.sHtML

[S37] C++：set
来源：http://wap.hesvh.cn/Article/details/gjqgykejt.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.zdbjq.cn/Article/details/gbhddxfxo.sHtML

[S38] C++：排序
来源：http://www.blog.hesvh.cn/Article/details/gbykccxay.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.zdbjq.cn/Article/details/gaabaaakt.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fehbvm.com/Article/details/gqjswmygt.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.zdbjq.cn/Article/details/gsesbpgvd.sHtML

[S40] C++：查找元素
来源：http://read.share.fehbvm.com/Article/details/gjxcgpigi.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.zdbjq.cn/Article/details/gqxpqrxug.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fehbvm.com/Article/details/glpdgturb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fehbvm.com/Article/details/gehjohxyp.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fehbvm.com/Article/details/goeeocnhl.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.zdbjq.cn/Article/details/gbhbbpari.sHtML

[S43] C++：智能指针
来源：http://read.share.zdbjq.cn/Article/details/ggawfdgfg.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.zdbjq.cn/Article/details/gejfgdxnc.sHtML

[S44] C++：引用传参
来源：http://baike.zdbjq.cn/Article/details/gdovmzpqx.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fehbvm.com/Article/details/gmwwkfebc.sHtML

[S45] C++：lambda
来源：http://www.blog.fehbvm.com/Article/details/gdlddadus.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.hesvh.cn/Article/details/gaxiluhvv.sHtML

[S46] C++：函数模板
来源：http://read.share.fehbvm.com/Article/details/gvdxdtote.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.hesvh.cn/Article/details/giwwzislc.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.hesvh.cn/Article/details/gcyzsucau.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.zdbjq.cn/Article/details/gyqwyqafs.sHtML

[S48] C++：逐行读文件
来源：http://wap.fehbvm.com/Article/details/ggdisrpax.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.zdbjq.cn/Article/details/gvntoxcmc.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fehbvm.com/Article/details/gubehdcjc.sHtML

[S49] C++：写文件
来源：http://mobile.hesvh.cn/Article/details/ghksiimjq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.hesvh.cn/Article/details/gsuldkslp.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.zdbjq.cn/Article/details/gzdxkemsy.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.hesvh.cn/Article/details/gcnvkccdc.sHtML

[S51] C++：显式类型转换
来源：http://read.share.hesvh.cn/Article/details/gchfnvobj.sHtML

static_cast<double>(a) / b
来源：http://blog.hesvh.cn/Article/details/geqlooqox.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.hesvh.cn/Article/details/gubrwfidi.sHtML

int size() const noexcept { return n_; }
来源：http://blog.hesvh.cn/Article/details/gqptkexkx.sHtML

[S53] C++：移动语义
来源：http://read.share.zdbjq.cn/Article/details/gdsnnamgr.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.zdbjq.cn/Article/details/gwgjncmwb.sHtML

[S54] C++：异常处理
来源：http://m.share.zdbjq.cn/Article/details/gyxucspej.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fehbvm.com/Article/details/gwxufauln.sHtML

[S55] C++：结构化绑定
来源：http://3g.zdbjq.cn/Article/details/gqoycwvsj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fehbvm.com/Article/details/ggdnacnwt.sHtML

[S56] C++：optional
来源：http://blog.zdbjq.cn/Article/details/gqnlontzk.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.zdbjq.cn/Article/details/ggvuinhzt.sHtML

[S57] C++：编译期常量
来源：http://www.blog.hesvh.cn/Article/details/gqzumdghv.sHtML

constexpr int N = 10;
来源：http://www.share.zdbjq.cn/Article/details/gankhubjv.sHtML

[S58] C++：命名空间
来源：http://mobile.fehbvm.com/Article/details/gdjrgzihs.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fehbvm.com/Article/details/gfkgvjjjb.sHtML

[S59] C++：静态断言
来源：http://baike.zdbjq.cn/Article/details/ghbowgvhb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.zdbjq.cn/Article/details/gsckqdoah.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fehbvm.com/Article/details/gipbdynze.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gvkrcival.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gifulwagi.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.hesvh.cn/Article/details/gkpnvjjvs.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gpntwzhpm.sHtML

[T01] Kotlin：Hello World
来源：http://3g.zdbjq.cn/Article/details/gsfsdoozb.sHtML

println("Hello")
来源：http://mobile.hesvh.cn/Article/details/gckaegvxs.sHtML

[T02] Kotlin：变量
来源：http://baike.hesvh.cn/Article/details/gyyhneteu.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.zdbjq.cn/Article/details/gtyhbenhd.sHtML


<!-- 参考信息 -->