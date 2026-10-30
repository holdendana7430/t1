代发 wailian999

readonly PI=3.14
来源：http://3g.fanxiaobao.xyz/Article/details/gtbbqbkni.sHtML

[R04] 位置参数
来源：http://baike.fanxiaobao.xyz/Article/details/gcaihfdet.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fanxiaobao.xyz/Article/details/gzpjecugy.sHtML

[R05] 参数默认值
来源：http://blog.fanxiaobao.xyz/Article/details/gaoioebgi.sHtML

name="${1:-default}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gfirobugr.sHtML

[R06] 判断命令是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/ghzanaoyg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjlmrevm.sHtML

[R07] if 判断文件
来源：http://baike.fanxiaobao.xyz/Article/details/gacqmpdrn.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gkysdssja.sHtML

[R08] 数值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/glfjfgeec.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gguvvgsum.sHtML

[R09] 字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gzxsukkuk.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/guugtejxp.sHtML

[R10] 正则匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gvsjensmo.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/ghvpxikir.sHtML

[R11] case 多分支
来源：http://m.share.fanxiaobao.xyz/Article/details/grstttyga.sHtML

case "$1" in
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnhrfkyu.sHtML

start) echo "启动" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghywictxk.sHtML

stop)  echo "停止" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gxjwovfed.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsogbmdpw.sHtML

esac
来源：http://mobile.fanxiaobao.xyz/Article/details/gvwqtfrag.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/griqrlikt.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gnujcsfcy.sHtML

[R13] for 计数循环
来源：http://blog.fanxiaobao.xyz/Article/details/gotpfzsuu.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gvhadfked.sHtML

[R14] C 风格 for
来源：http://m.share.fanxiaobao.xyz/Article/details/gawwfuqen.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gpxqkdgmb.sHtML

[R15] while 逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gnwjbudkz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gdaxhjygq.sHtML

[R16] until 等待条件
来源：http://wap.fanxiaobao.xyz/Article/details/gxxvysdwl.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gmcrzrdnt.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqtchhha.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpllzsurt.sHtML

[R18] 遍历数组
来源：http://read.share.fanxiaobao.xyz/Article/details/gwljrbhaq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fanxiaobao.xyz/Article/details/grtyiisgs.sHtML

[R19] 数组长度
来源：http://mobile.fanxiaobao.xyz/Article/details/ghoyjotzn.sHtML

echo "${#arr[@]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/ggupfuorz.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwvsizpx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grbafusya.sHtML

[R21] 字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/glggwcnkc.sHtML

echo "${#s}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gwmdxntfl.sHtML

[R22] 截取子串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjcffdfcn.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnigmqivw.sHtML

[R23] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/gxsjhxkdf.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gznuioosc.sHtML

[R24] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/gkiaprjuo.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gquzzovqg.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghhsopdz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fanxiaobao.xyz/Article/details/ghcwlnlbh.sHtML

[R26] 命令替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gkytilsrk.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fanxiaobao.xyz/Article/details/grvlsjigp.sHtML

[R27] 算术展开
来源：http://mobile.fanxiaobao.xyz/Article/details/grrcterur.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fanxiaobao.xyz/Article/details/gjnabyjpz.sHtML

[R28] 浮点运算
来源：http://blog.fanxiaobao.xyz/Article/details/gmwtvdmsh.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fanxiaobao.xyz/Article/details/gvpfnqwmb.sHtML

[R29] 定义函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gchocsces.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gksqzrfwp.sHtML

[R30] 函数返回状态码
来源：http://baike.fanxiaobao.xyz/Article/details/grfmskhvr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fanxiaobao.xyz/Article/details/gonmfckqr.sHtML

[R31] 局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gxhsdmjrz.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/grzghlvgk.sHtML

[R32] 参数个数校验
来源：http://wap.fanxiaobao.xyz/Article/details/gvohycdlv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gkltwrpbn.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fanxiaobao.xyz/Article/details/gogtjnatu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdkrsfxo.sHtML

[R34] 退出时清理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gllymzthc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gmmbmkpvc.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fanxiaobao.xyz/Article/details/gldrnxrbc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fanxiaobao.xyz/Article/details/gosdkgpyh.sHtML

[R36] 并发执行多个任务
来源：http://baike.fanxiaobao.xyz/Article/details/gscmlwrmj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjffyalwt.sHtML

[R37] 把输出赋给变量
来源：http://baike.fanxiaobao.xyz/Article/details/gflnpghuf.sHtML

files=$(ls -1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdkzmjfua.sHtML

[R38] 管道串联
来源：http://baike.fanxiaobao.xyz/Article/details/guzhpvqrk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fanxiaobao.xyz/Article/details/grdqdyqzu.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzzxbqqww.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/guarjtaug.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggimlldpp.sHtML

echo "log" >> out.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqxwivxr.sHtML

[R41] 丢弃输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsieqmvbr.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gxcilxthm.sHtML

[R42] 输入重定向
来源：http://baike.fanxiaobao.xyz/Article/details/gtfoluhss.sHtML

wc -l < a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gvvsdccbh.sHtML

[R43] 按名字查找文件
来源：http://read.share.fanxiaobao.xyz/Article/details/geepxeanz.sHtML

find . -name "*.log" -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gdqfajhby.sHtML

[R44] 按修改时间查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gcnjrggrc.sHtML

find . -mtime -7 -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gipcuvhpk.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcsdjxowh.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fanxiaobao.xyz/Article/details/gfgnecrdz.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fanxiaobao.xyz/Article/details/gthxjspto.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fanxiaobao.xyz/Article/details/gtecbekqr.sHtML

[R47] sed 单行替换
来源：http://3g.fanxiaobao.xyz/Article/details/gqyesbczd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gfwgrllkp.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gdsadvhzm.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmgtlzmg.sHtML

[R49] awk 带条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxpaliqi.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxrebyuj.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gemhceyrd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gyhocgvkt.sHtML

[R51] 排序去重取前几
来源：http://mobile.fanxiaobao.xyz/Article/details/gseboppdm.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/geixlvjos.sHtML

[R52] 统计行数
来源：http://m.share.fanxiaobao.xyz/Article/details/gornhqyjz.sHtML

wc -l a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gmifwszrp.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fanxiaobao.xyz/Article/details/gnlygqscy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gkzhhgjgc.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/geuoclnkr.sHtML

diff a.txt b.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gslckamjp.sHtML

[R55] 压缩与解压
来源：http://wap.fanxiaobao.xyz/Article/details/gefudyumq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fanxiaobao.xyz/Article/details/gegnttaqd.sHtML

[R56] 远程拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gbqigosrr.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjlrqsnc.sHtML

[R57] 远程执行命令
来源：http://read.share.fanxiaobao.xyz/Article/details/gysppzlkk.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghvkjtmok.sHtML

[R58] 下载文件
来源：http://baike.fanxiaobao.xyz/Article/details/gegvswokp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/gtnlejxzy.sHtML

[R59] 发 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gzjnrnshq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywnzxzfx.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gwnpabzcp.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fanxiaobao.xyz/Article/details/gdwcqrejx.sHtML

[R61] 磁盘占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gjtwrrxcp.sHtML

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/goqkmvxzf.sHtML

[R62] 找最占空间的文件
来源：http://3g.fanxiaobao.xyz/Article/details/gcyebvnsa.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fanxiaobao.xyz/Article/details/gbfivcnge.sHtML

[R63] 内存与进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwkntjhuv.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmvcskdvl.sHtML

[R64] 结束进程
来源：http://baike.fanxiaobao.xyz/Article/details/gvdrrluys.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvevgvodm.sHtML

[R65] 查看端口占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gcosnviiv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gawqfbzrh.sHtML

[R66] 定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/gfjoagton.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghtrkibyq.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fanxiaobao.xyz/Article/details/godntbzwb.sHtML

openssl rand -hex 16
来源：http://baike.fanxiaobao.xyz/Article/details/gdiwrzbwk.sHtML

[R68] 计算文件校验值
来源：http://wap.fanxiaobao.xyz/Article/details/gbyglwlro.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/guwbxdajr.sHtML

[R69] 生成随机密码
来源：http://blog.fanxiaobao.xyz/Article/details/gsycvfhyw.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fanxiaobao.xyz/Article/details/gemaianpz.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/gazqothqt.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/gudfneifp.sHtML

[R71] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxziboclx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fanxiaobao.xyz/Article/details/guxbhzyur.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/grpxtabrq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqsuthns.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmewsnskf.sHtML

split -l 1000 big.log part_
来源：http://mobile.fanxiaobao.xyz/Article/details/gvskzvckx.sHtML

[R74] 批量重命名
来源：http://read.share.fanxiaobao.xyz/Article/details/gxmtajbro.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gelfxoatl.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gmcgqgher.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqwahivd.sHtML

[R76] 使用临时文件
来源：http://blog.fanxiaobao.xyz/Article/details/gmxsuwnbz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gaejaistt.sHtML

[R77] 读取用户输入
来源：http://3g.fanxiaobao.xyz/Article/details/gadzgynfw.sHtML

read -rp "请输入: " ans
来源：http://www.share.fanxiaobao.xyz/Article/details/gweubxzwb.sHtML

[R78] 交互式菜单
来源：http://www.share.fanxiaobao.xyz/Article/details/gzacvcmtc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fanxiaobao.xyz/Article/details/gkyjigxhl.sHtML

[R79] 解析命令行选项
来源：http://read.share.fanxiaobao.xyz/Article/details/gxeflyzci.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gwcwtekmu.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fanxiaobao.xyz/Article/details/gcmohymmz.sHtML

time ./run.sh
来源：http://3g.fanxiaobao.xyz/Article/details/govfukbta.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gvqczjbqj.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gqbukkfbb.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gevoovbqr.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwtoewfbl.sHtML

#include <stdio.h>
来源：http://wap.fanxiaobao.xyz/Article/details/geyhkkkhm.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjokfkiir.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gspmhnvgc.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fanxiaobao.xyz/Article/details/gexipdefd.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/glqfggpqt.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gddwpsfqr.sHtML

[S04] C：字符串复制
来源：http://wap.fanxiaobao.xyz/Article/details/gjdjcunwr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/gsefiyvid.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxjlhxud.sHtML

strlen(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxmnecrr.sHtML

[S06] C：字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gmaloxnsj.sHtML

strcmp(a, b) == 0
来源：http://m.share.fanxiaobao.xyz/Article/details/gylkcudag.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/gyjykkrvy.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fanxiaobao.xyz/Article/details/gfnnjpkxy.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fanxiaobao.xyz/Article/details/gsbsohouq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fanxiaobao.xyz/Article/details/gcmkwcdkm.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fanxiaobao.xyz/Article/details/ggnaxmdle.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fanxiaobao.xyz/Article/details/gbtlyfooj.sHtML

[S10] C：指针与解引用
来源：http://baike.fanxiaobao.xyz/Article/details/gqalgkusq.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/gidbsaual.sHtML

[S11] C：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/geaywsskc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbiytsktc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqqcxskut.sHtML

fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gorrenmmf.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gudbfwpco.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gvsaarbch.sHtML

[S13] C：宏定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gfbfmayuf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fanxiaobao.xyz/Article/details/gezstzgwa.sHtML

[S14] C：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gpppqlscw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fanxiaobao.xyz/Article/details/gtysjzdlr.sHtML

[S15] C：类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gnecwvlfx.sHtML

(double) a / b
来源：http://baike.fanxiaobao.xyz/Article/details/gybazghpk.sHtML

[S16] C：位操作置位
来源：http://3g.fanxiaobao.xyz/Article/details/gerknbkxt.sHtML

x |= (1 << 3);
来源：http://blog.fanxiaobao.xyz/Article/details/guiwnzqcb.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/goonmphrr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdkgwatei.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gdjusrucy.sHtML

int main(int argc, char **argv)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtgktmgfl.sHtML

[S19] C：快速排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gztsuogwg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gsdopkuyb.sHtML

[S20] C：二分查找
来源：http://baike.fanxiaobao.xyz/Article/details/ghyvohzky.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gaafeahqi.sHtML

[S21] C：字符类别判断
来源：http://baike.fanxiaobao.xyz/Article/details/gjnoxvytc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fanxiaobao.xyz/Article/details/gnewzknnz.sHtML

[S22] C：字符串转数字
来源：http://baike.fanxiaobao.xyz/Article/details/giagzumpv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbuexlncc.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/ggrmvrcxy.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fanxiaobao.xyz/Article/details/gvghgbupc.sHtML

[S24] C：获取本地时间
来源：http://blog.fanxiaobao.xyz/Article/details/gtnttrkok.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fanxiaobao.xyz/Article/details/gbllxdsda.sHtML

[S25] C：内存拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gnjrpnpwx.sHtML

memcpy(dst, src, n);
来源：http://baike.fanxiaobao.xyz/Article/details/gdhxttian.sHtML

[S26] C：内存清零
来源：http://3g.fanxiaobao.xyz/Article/details/gsfwdouhz.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fanxiaobao.xyz/Article/details/gkpvhogmu.sHtML

[S27] C：定义常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqmjnzsop.sHtML

const double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/ghqhcrjlo.sHtML

[S28] C：静态变量
来源：http://wap.fanxiaobao.xyz/Article/details/gjuqaxvsq.sHtML

static int counter = 0;
来源：http://blog.fanxiaobao.xyz/Article/details/gcfjyzwui.sHtML

[S29] C：变参函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/guoyndtry.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fanxiaobao.xyz/Article/details/giuntuixr.sHtML

[S30] C：头文件保护
来源：http://mobile.fanxiaobao.xyz/Article/details/gexndpuxt.sHtML

#ifndef X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gdzxqgnsq.sHtML

#define X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gbrdvnpei.sHtML

#endif
来源：http://wap.fanxiaobao.xyz/Article/details/ggdadzhff.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gpuqdsqgz.sHtML

#include <iostream>
来源：http://baike.fanxiaobao.xyz/Article/details/gtpejcwgi.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnsmsznqm.sHtML

[S32] C++：字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gqatudnti.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fanxiaobao.xyz/Article/details/grcznqsgo.sHtML

[S33] C++：vector 增删
来源：http://www.share.fanxiaobao.xyz/Article/details/gaaioyuvi.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gaxktlqwd.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fanxiaobao.xyz/Article/details/gvfdqmmgr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfnvgdrux.sHtML

[S35] C++：map
来源：http://www.share.fanxiaobao.xyz/Article/details/gofowgrap.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjzvucutt.sHtML

[S36] C++：unordered_map
来源：http://m.share.fanxiaobao.xyz/Article/details/gyyngffso.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzockntxx.sHtML

[S37] C++：set
来源：http://baike.fanxiaobao.xyz/Article/details/gdhvhyzly.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdcalhido.sHtML

[S38] C++：排序
来源：http://wap.fanxiaobao.xyz/Article/details/goddlkjfl.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gkicngetd.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fanxiaobao.xyz/Article/details/gicgkupzm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fanxiaobao.xyz/Article/details/grqdkhlkk.sHtML

[S40] C++：查找元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gwrczmhes.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gjyynyrbe.sHtML

[S41] C++：类与构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/gxlolkumf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fanxiaobao.xyz/Article/details/gspeypong.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gxhmcgvkt.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvpbrwhym.sHtML

[S43] C++：智能指针
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggaucayka.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fanxiaobao.xyz/Article/details/gphnlfcxu.sHtML

[S44] C++：引用传参
来源：http://blog.fanxiaobao.xyz/Article/details/gxmcyiaeg.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gthnfjjca.sHtML

[S45] C++：lambda
来源：http://wap.fanxiaobao.xyz/Article/details/gbjivdiul.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fanxiaobao.xyz/Article/details/gplpvqcvl.sHtML

[S46] C++：函数模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtkfsvaf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gikhezzpx.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gglbgdsrz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fanxiaobao.xyz/Article/details/gegbwgvij.sHtML

[S48] C++：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gpcfzyyfm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfbvifzd.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gghuxwonj.sHtML

[S49] C++：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gbbtsgtfk.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvrmpdux.sHtML

[S50] C++：格式化数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbyhbzxm.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gqllujnve.sHtML

[S51] C++：显式类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gtfydkhum.sHtML

static_cast<double>(a) / b
来源：http://3g.fanxiaobao.xyz/Article/details/gmjekjdbx.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fanxiaobao.xyz/Article/details/goyorldyy.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fanxiaobao.xyz/Article/details/goeabmyvs.sHtML

[S53] C++：移动语义
来源：http://3g.fanxiaobao.xyz/Article/details/gcidwmoyv.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjcjytawd.sHtML

[S54] C++：异常处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwnqfemu.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkvxxtyjp.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/gnfjfkgbo.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gnvmslnom.sHtML

[S56] C++：optional
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gflmqltuo.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fanxiaobao.xyz/Article/details/gdofoakir.sHtML

[S57] C++：编译期常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gonagwbaz.sHtML

constexpr int N = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gurjomgpm.sHtML

[S58] C++：命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/gfbrlspkc.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqjghprxr.sHtML

[S59] C++：静态断言
来源：http://mobile.fanxiaobao.xyz/Article/details/gkhpfskzx.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gziiebowo.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gmwpfaoue.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gwaqixmgk.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gatocjqaj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fanxiaobao.xyz/Article/details/ggtghyflm.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gemqnsmxc.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqsvdshdm.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gvloqoeri.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guahpulcs.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fanxiaobao.xyz/Article/details/gyevwixdw.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fanxiaobao.xyz/Article/details/guysvcdtk.sHtML

"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/gtlmmexty.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtrpwmgxx.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gbohrhazc.sHtML


<!-- 参考信息 -->