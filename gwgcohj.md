代发 wailian999

name="${1:-default}"
来源：http://3g.fanxiaobao.xyz/Article/details/gpsxiokdr.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gpnszxpfl.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gdqlojaas.sHtML

[R07] if 判断文件
来源：http://wap.fanxiaobao.xyz/Article/details/gkdculdxu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gjqxtsghl.sHtML

[R08] 数值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gqbkaearz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gsqzgithm.sHtML

[R09] 字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gioavymju.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gyjdvqiba.sHtML

[R10] 正则匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/grevpcyxl.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/ggugftmbj.sHtML

[R11] case 多分支
来源：http://blog.fanxiaobao.xyz/Article/details/gbzgkmsve.sHtML

case "$1" in
来源：http://mobile.fanxiaobao.xyz/Article/details/ghexqawyo.sHtML

start) echo "启动" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gjgseybot.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxwtaodma.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfobahngt.sHtML

esac
来源：http://baike.fanxiaobao.xyz/Article/details/gshoatrsc.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcuwugbdc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gjdrvolzl.sHtML

[R13] for 计数循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gticragbi.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvduqgtxl.sHtML

[R14] C 风格 for
来源：http://m.share.fanxiaobao.xyz/Article/details/gkekiaxql.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/ghzcmffwo.sHtML

[R15] while 逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gcteetpqw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gojdzpogy.sHtML

[R16] until 等待条件
来源：http://baike.fanxiaobao.xyz/Article/details/gvmhyszlu.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfxpwpifk.sHtML

[R17] 数组定义与取值
来源：http://read.share.fanxiaobao.xyz/Article/details/gvaddbuhl.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gjegvxhwa.sHtML

[R18] 遍历数组
来源：http://wap.fanxiaobao.xyz/Article/details/gsjocivef.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gqbgmotnf.sHtML

[R19] 数组长度
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnyzvnen.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzwlqlyzv.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fanxiaobao.xyz/Article/details/gpvauvmnr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdkmeygug.sHtML

[R21] 字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gihsvhddf.sHtML

echo "${#s}"
来源：http://blog.fanxiaobao.xyz/Article/details/ggqnhahws.sHtML

[R22] 截取子串
来源：http://mobile.fanxiaobao.xyz/Article/details/gzcfceijz.sHtML

echo "${s:0:5}"
来源：http://blog.fanxiaobao.xyz/Article/details/ggheirhbw.sHtML

[R23] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glxwhzqfs.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/guixdvnnb.sHtML

[R24] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gexnxvpnt.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fanxiaobao.xyz/Article/details/gmbgswzut.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fanxiaobao.xyz/Article/details/gljqeoodr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsnseedpa.sHtML

[R26] 命令替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gyaiznlvj.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjclmydyd.sHtML

[R27] 算术展开
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmnfqikna.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/gqrjnsipk.sHtML

[R28] 浮点运算
来源：http://m.share.fanxiaobao.xyz/Article/details/geltlgfmx.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqwhvarvz.sHtML

[R29] 定义函数
来源：http://wap.fanxiaobao.xyz/Article/details/gstdzzads.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fanxiaobao.xyz/Article/details/ghirhrmjs.sHtML

[R30] 函数返回状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gqufthzwf.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fanxiaobao.xyz/Article/details/gcmndfzln.sHtML

[R31] 局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gklutrjml.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjpgewqpq.sHtML

[R32] 参数个数校验
来源：http://baike.fanxiaobao.xyz/Article/details/glgmghsgq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxyglrgjl.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gmujloyeu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmxjizzp.sHtML

[R34] 退出时清理
来源：http://baike.fanxiaobao.xyz/Article/details/gpqcsmxuf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/graocrdxd.sHtML

[R35] 后台执行并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxityngb.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fanxiaobao.xyz/Article/details/gspluiajl.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehzlpnyv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giyyjbold.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwttrvgp.sHtML

files=$(ls -1)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghxcxuzcz.sHtML

[R38] 管道串联
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojulzhou.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fanxiaobao.xyz/Article/details/giqmbtcnl.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fanxiaobao.xyz/Article/details/guppmpmao.sHtML

cmd > out.log 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gpaxbrhmk.sHtML

[R40] 追加写日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gadqpoezm.sHtML

echo "log" >> out.log
来源：http://baike.fanxiaobao.xyz/Article/details/gfvuxlbrd.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gibqgkrxi.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gdoumigpj.sHtML

[R42] 输入重定向
来源：http://mobile.fanxiaobao.xyz/Article/details/gbkwyzyey.sHtML

wc -l < a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gtpwjjasd.sHtML

[R43] 按名字查找文件
来源：http://3g.fanxiaobao.xyz/Article/details/gesmxvqwt.sHtML

find . -name "*.log" -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gxxhcvure.sHtML

[R44] 按修改时间查找
来源：http://wap.fanxiaobao.xyz/Article/details/gxrtwaoqu.sHtML

find . -mtime -7 -type f
来源：http://wap.fanxiaobao.xyz/Article/details/grtrrzeqn.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/gyemuvsrl.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giymfvrog.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fanxiaobao.xyz/Article/details/gveutahdt.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govgidzcm.sHtML

[R47] sed 单行替换
来源：http://wap.fanxiaobao.xyz/Article/details/gsitzyixf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gswkmsuge.sHtML

[R48] awk 取指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyqrliztp.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gpdxsgqbh.sHtML

[R49] awk 带条件
来源：http://3g.fanxiaobao.xyz/Article/details/gmctxjmkc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/gdzocxoff.sHtML

[R50] awk 求和
来源：http://wap.fanxiaobao.xyz/Article/details/gngtshnhk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gkjeyxeab.sHtML

[R51] 排序去重取前几
来源：http://read.share.fanxiaobao.xyz/Article/details/glymuqyjj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/grnvtxhsl.sHtML

[R52] 统计行数
来源：http://baike.fanxiaobao.xyz/Article/details/gjgyhhwkc.sHtML

wc -l a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gctpmjxyp.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fanxiaobao.xyz/Article/details/gmrgpetod.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gjhzsaeqx.sHtML

[R54] 比较两个文件
来源：http://3g.fanxiaobao.xyz/Article/details/gpfzmvtgx.sHtML

diff a.txt b.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/glhxnceec.sHtML

[R55] 压缩与解压
来源：http://m.share.fanxiaobao.xyz/Article/details/geelqhmin.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggyvrqaxu.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gikfxpjvr.sHtML

scp file user@host:/path/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggavffabs.sHtML

[R57] 远程执行命令
来源：http://baike.fanxiaobao.xyz/Article/details/gbngutzck.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpsjqklet.sHtML

[R58] 下载文件
来源：http://wap.fanxiaobao.xyz/Article/details/gqdnuezjz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcgjufwlj.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtsjmfqmp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjqybmbet.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gnkehskro.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fanxiaobao.xyz/Article/details/glggqkwcn.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gieqmkecd.sHtML

df -h;  du -sh *
来源：http://blog.fanxiaobao.xyz/Article/details/gdadbxyqs.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gvkwuklvf.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fanxiaobao.xyz/Article/details/gkmyxugif.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gvqzubalv.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fanxiaobao.xyz/Article/details/gclslhtwc.sHtML

[R64] 结束进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gxtrhseto.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fanxiaobao.xyz/Article/details/gnjycnncv.sHtML

[R65] 查看端口占用
来源：http://read.share.fanxiaobao.xyz/Article/details/goyfsanzp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fanxiaobao.xyz/Article/details/gonfmusis.sHtML

[R66] 定时任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzrchqjqa.sHtML

crontab -e;  crontab -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gtxdcmnih.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fanxiaobao.xyz/Article/details/goppvvkgm.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/gtxknsvcj.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvytajfei.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gbncmpdlz.sHtML

[R69] 生成随机密码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvkpcmkag.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxagjifq.sHtML

[R70] 时间戳与互转
来源：http://m.share.fanxiaobao.xyz/Article/details/gqlxdcxtc.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fanxiaobao.xyz/Article/details/gfrwdznuu.sHtML

[R71] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/ghbaxxcim.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fanxiaobao.xyz/Article/details/gzihiujtw.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/gpnlagpvg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/guumjcuoz.sHtML

[R73] 分割大日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gnlbzhjte.sHtML

split -l 1000 big.log part_
来源：http://mobile.fanxiaobao.xyz/Article/details/gguyljmjl.sHtML

[R74] 批量重命名
来源：http://www.share.fanxiaobao.xyz/Article/details/gpzbhrlaw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gvivswopm.sHtML

[R75] 导出环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/gsrxwmatp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqtixflo.sHtML

[R76] 使用临时文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gwnlhnalh.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gscwypoig.sHtML

[R77] 读取用户输入
来源：http://www.share.fanxiaobao.xyz/Article/details/gfzdbcejr.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/gyniqauom.sHtML

[R78] 交互式菜单
来源：http://www.share.fanxiaobao.xyz/Article/details/groawjaoy.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fanxiaobao.xyz/Article/details/gswnmkpxs.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giczunibf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grhrzgudb.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fanxiaobao.xyz/Article/details/gvljsdmxz.sHtML

time ./run.sh
来源：http://wap.fanxiaobao.xyz/Article/details/gpdwapoua.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/glcwvcvbq.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gvpelvwtx.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gerufffie.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjkwxagej.sHtML

#include <stdio.h>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdwkmgryg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fanxiaobao.xyz/Article/details/gttnxhkeh.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghcxmdujy.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnzatakoa.sHtML

[S03] C：读入整数
来源：http://wap.fanxiaobao.xyz/Article/details/gntfmidcw.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fanxiaobao.xyz/Article/details/gobaydkjf.sHtML

[S04] C：字符串复制
来源：http://read.share.fanxiaobao.xyz/Article/details/gtseegrrx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gralynvoe.sHtML

[S05] C：字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gfhmzbamw.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gowcqyrvs.sHtML

[S06] C：字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gmqmtbmjv.sHtML

strcmp(a, b) == 0
来源：http://m.share.fanxiaobao.xyz/Article/details/gtzuzejev.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/gxwrotsfo.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fanxiaobao.xyz/Article/details/gzhxxulmn.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fanxiaobao.xyz/Article/details/geoakohbc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzhxorvxx.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fanxiaobao.xyz/Article/details/gwzoxiiol.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fanxiaobao.xyz/Article/details/gjhrrvjbu.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gikqauhup.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/ggpdnllva.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqzhqvyg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fanxiaobao.xyz/Article/details/gpcioedrs.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/goaylstbk.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grjgdyxfl.sHtML

[S12] C：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghkqyetmg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gmcrlsznb.sHtML

[S13] C：宏定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gishthqtn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fanxiaobao.xyz/Article/details/gngwasxah.sHtML

[S14] C：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gakwilfns.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fanxiaobao.xyz/Article/details/gunpxxzwn.sHtML

[S15] C：类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gwptpsvyh.sHtML

(double) a / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glinkzmif.sHtML

[S16] C：位操作置位
来源：http://blog.fanxiaobao.xyz/Article/details/gngfanrkm.sHtML

x |= (1 << 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gcvmdsrxs.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdavujbd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpjwwmfap.sHtML

[S18] C：命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/gziexewmi.sHtML

int main(int argc, char **argv)
来源：http://blog.fanxiaobao.xyz/Article/details/gdorfpary.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/gkimophno.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gxztumbnx.sHtML

[S20] C：二分查找
来源：http://blog.fanxiaobao.xyz/Article/details/gobfhuegy.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdhejnjwg.sHtML

[S21] C：字符类别判断
来源：http://baike.fanxiaobao.xyz/Article/details/gkyfoffat.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fanxiaobao.xyz/Article/details/gniiicfyl.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/gftvolbub.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fanxiaobao.xyz/Article/details/gmnfoxqnw.sHtML

[S23] C：随机数
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdnenqru.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fanxiaobao.xyz/Article/details/ggbzvablr.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaynknjbx.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnuamnnxu.sHtML

[S25] C：内存拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gqddsvmhc.sHtML

memcpy(dst, src, n);
来源：http://wap.fanxiaobao.xyz/Article/details/goeshovgj.sHtML

[S26] C：内存清零
来源：http://www.share.fanxiaobao.xyz/Article/details/gjxwpmvxc.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvekqfrsh.sHtML

[S27] C：定义常量
来源：http://wap.fanxiaobao.xyz/Article/details/gndrijyzs.sHtML

const double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxvqejpcq.sHtML

[S28] C：静态变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfqilthdq.sHtML

static int counter = 0;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzferjzta.sHtML

[S29] C：变参函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gqyoudwgc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvwyuzvdx.sHtML

[S30] C：头文件保护
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggwvidyey.sHtML

#ifndef X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghyaxjnhw.sHtML

#define X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gotcovuen.sHtML

#endif
来源：http://blog.fanxiaobao.xyz/Article/details/gvbrtfwon.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gpheygyvu.sHtML

#include <iostream>
来源：http://baike.fanxiaobao.xyz/Article/details/gqrogxkwp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fanxiaobao.xyz/Article/details/goslhgsyz.sHtML

[S32] C++：字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/giehyleaz.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fanxiaobao.xyz/Article/details/gizabyohv.sHtML

[S33] C++：vector 增删
来源：http://3g.fanxiaobao.xyz/Article/details/gqefrqwbm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gereecgry.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fanxiaobao.xyz/Article/details/gfowivrua.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gesapopze.sHtML

[S35] C++：map
来源：http://blog.fanxiaobao.xyz/Article/details/ghbekweih.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gubwyragv.sHtML

[S36] C++：unordered_map
来源：http://3g.fanxiaobao.xyz/Article/details/ggbnzjlls.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gortetrhp.sHtML

[S37] C++：set
来源：http://www.blog.fanxiaobao.xyz/Article/details/guwkcvkbb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gayzmdupb.sHtML

[S38] C++：排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gifokxgqm.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gfnkxeciv.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fanxiaobao.xyz/Article/details/gmkrjhopi.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzbwyjaia.sHtML

[S40] C++：查找元素
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqmmtidz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glrfqpblq.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gznfbivjz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gkkykhcxx.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fanxiaobao.xyz/Article/details/gfwpqirnc.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/gfvusveuw.sHtML

[S43] C++：智能指针
来源：http://3g.fanxiaobao.xyz/Article/details/gketmugrt.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsibqmxql.sHtML

[S44] C++：引用传参
来源：http://baike.fanxiaobao.xyz/Article/details/gdoshbngw.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gaikyxbou.sHtML

[S45] C++：lambda
来源：http://wap.fanxiaobao.xyz/Article/details/gxzltdbaj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fanxiaobao.xyz/Article/details/glurqzdbk.sHtML

[S46] C++：函数模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gpufefhba.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjufkzvxy.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gatgwyhja.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpsmviuwf.sHtML

[S48] C++：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gbucoejqm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwqyvops.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtpptfyn.sHtML

[S49] C++：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/goybmvrjv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkboycllh.sHtML

[S50] C++：格式化数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gyatjmxtv.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gxnvzzmig.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqjyqjrf.sHtML

static_cast<double>(a) / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbmlcalu.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fanxiaobao.xyz/Article/details/gdulrxjwg.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggqmwkebe.sHtML

[S53] C++：移动语义
来源：http://blog.fanxiaobao.xyz/Article/details/gkzhjhpqm.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfpskyfmz.sHtML

[S54] C++：异常处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggpyieuuj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gliyivpvb.sHtML

[S55] C++：结构化绑定
来源：http://baike.fanxiaobao.xyz/Article/details/gncwnktlb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fanxiaobao.xyz/Article/details/gvwouzmjp.sHtML

[S56] C++：optional
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxihatqt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fanxiaobao.xyz/Article/details/gfelwrnvt.sHtML

[S57] C++：编译期常量
来源：http://blog.fanxiaobao.xyz/Article/details/gbvnplgro.sHtML

constexpr int N = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfyesoafx.sHtML

[S58] C++：命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/gwpicekli.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzuujdtwj.sHtML

[S59] C++：静态断言
来源：http://3g.fanxiaobao.xyz/Article/details/gpfrxqimk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fanxiaobao.xyz/Article/details/gprumatoj.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdnmaqpkp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/grofmjzkh.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwqsvguvf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fanxiaobao.xyz/Article/details/gzmvnarzn.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gldzmhewt.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gtomjrovt.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/grycbeksf.sHtML

[T02] Kotlin：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/grfhzmceo.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fanxiaobao.xyz/Article/details/gawbccxog.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gvebnntgf.sHtML

"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/ghxmhtoiu.sHtML

[T04] Kotlin：空安全
来源：http://wap.fanxiaobao.xyz/Article/details/geyfxrjmt.sHtML

val n: String? = null;  n?.length
来源：http://blog.fanxiaobao.xyz/Article/details/gcjqichsh.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gbgvqfqjp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fanxiaobao.xyz/Article/details/gzeqohghm.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/gblxybydm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gdlnvbtpm.sHtML


<!-- 参考信息 -->