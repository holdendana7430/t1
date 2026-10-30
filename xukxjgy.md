代发 wailian999

esac
来源：http://read.share.fanxiaobao.xyz/Article/details/gpcrwisej.sHtML

[R12] for 遍历文件
来源：http://www.share.fanxiaobao.xyz/Article/details/ghrhfpywo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gwgeghmzd.sHtML

[R13] for 计数循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbezhmcms.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gtlzvvegu.sHtML

[R14] C 风格 for
来源：http://www.blog.fanxiaobao.xyz/Article/details/gddoirkjn.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwivtktoo.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnzozgrwb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gckfcvxas.sHtML

[R16] until 等待条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpsubpsdf.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjnjsxhfl.sHtML

[R17] 数组定义与取值
来源：http://baike.fanxiaobao.xyz/Article/details/glvfddvyz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gvmblosud.sHtML

[R18] 遍历数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gdtbbspyw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fanxiaobao.xyz/Article/details/ghmkyhlxr.sHtML

[R19] 数组长度
来源：http://m.share.fanxiaobao.xyz/Article/details/grepvwaaq.sHtML

echo "${#arr[@]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gxajinytw.sHtML

[R20] 关联数组（字典）
来源：http://wap.fanxiaobao.xyz/Article/details/gxmfhswmo.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gtiedxusc.sHtML

[R21] 字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gsjsrpacm.sHtML

echo "${#s}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gbabkhpon.sHtML

[R22] 截取子串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gctgftbub.sHtML

echo "${s:0:5}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gvbihjgoj.sHtML

[R23] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/geyfiocjj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gofvkyfmz.sHtML

[R24] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gepaxoniq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhmhgoqp.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fanxiaobao.xyz/Article/details/gjzbufzbk.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fanxiaobao.xyz/Article/details/glhupbqqs.sHtML

[R26] 命令替换
来源：http://3g.fanxiaobao.xyz/Article/details/gipzyivjv.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fanxiaobao.xyz/Article/details/gunzanvba.sHtML

[R27] 算术展开
来源：http://mobile.fanxiaobao.xyz/Article/details/ggipainow.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/gcdayrdry.sHtML

[R28] 浮点运算
来源：http://www.share.fanxiaobao.xyz/Article/details/grgkueyww.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fanxiaobao.xyz/Article/details/gasvshvsz.sHtML

[R29] 定义函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gudwzjlic.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fanxiaobao.xyz/Article/details/gusddqbay.sHtML

[R30] 函数返回状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gsvwjwesv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fanxiaobao.xyz/Article/details/gwufvhlpf.sHtML

[R31] 局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/grwmoffvx.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gwqpsobfn.sHtML

[R32] 参数个数校验
来源：http://mobile.fanxiaobao.xyz/Article/details/ghzdiwjxh.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gkgunkbyz.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbwzvicyg.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdzldnqy.sHtML

[R34] 退出时清理
来源：http://www.share.fanxiaobao.xyz/Article/details/gnuxvnnik.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gybahufkx.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvpvnokxm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fanxiaobao.xyz/Article/details/ghorvuvyq.sHtML

[R36] 并发执行多个任务
来源：http://blog.fanxiaobao.xyz/Article/details/glyonwyuz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fanxiaobao.xyz/Article/details/gjecnqcfr.sHtML

[R37] 把输出赋给变量
来源：http://baike.fanxiaobao.xyz/Article/details/gvfbznpqh.sHtML

files=$(ls -1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbgczsiml.sHtML

[R38] 管道串联
来源：http://www.blog.fanxiaobao.xyz/Article/details/gitxxkpbf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fanxiaobao.xyz/Article/details/gmmtnnxde.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gmtjofzmb.sHtML

cmd > out.log 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gbmnqstbx.sHtML

[R40] 追加写日志
来源：http://baike.fanxiaobao.xyz/Article/details/guvpqyack.sHtML

echo "log" >> out.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyflfobti.sHtML

[R41] 丢弃输出
来源：http://wap.fanxiaobao.xyz/Article/details/ghcyzknzs.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gwzlxcslc.sHtML

[R42] 输入重定向
来源：http://wap.fanxiaobao.xyz/Article/details/gjwbyssqs.sHtML

wc -l < a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gpeeyujor.sHtML

[R43] 按名字查找文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gmrdfsidq.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gvuyyldha.sHtML

[R44] 按修改时间查找
来源：http://baike.fanxiaobao.xyz/Article/details/gxjvkqfdh.sHtML

find . -mtime -7 -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gtgmohxxc.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/grwrdjolg.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfdexukwa.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fanxiaobao.xyz/Article/details/geywlkhyp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fanxiaobao.xyz/Article/details/gcioqdxup.sHtML

[R47] sed 单行替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gnhwauzex.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gdolbsxyg.sHtML

[R48] awk 取指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/gfjmtjyix.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gphqgpyws.sHtML

[R49] awk 带条件
来源：http://blog.fanxiaobao.xyz/Article/details/gxesmvlix.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fanxiaobao.xyz/Article/details/grauurqob.sHtML

[R50] awk 求和
来源：http://wap.fanxiaobao.xyz/Article/details/gnlamchfz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gyrvavsnj.sHtML

[R51] 排序去重取前几
来源：http://read.share.fanxiaobao.xyz/Article/details/glunkfjjs.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fanxiaobao.xyz/Article/details/gfctakkia.sHtML

[R52] 统计行数
来源：http://m.share.fanxiaobao.xyz/Article/details/gjjexmdhc.sHtML

wc -l a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gqvjfaqzt.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fanxiaobao.xyz/Article/details/gbpgcrhma.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fanxiaobao.xyz/Article/details/guopzhozr.sHtML

[R54] 比较两个文件
来源：http://3g.fanxiaobao.xyz/Article/details/gfbowahge.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gknvekaxh.sHtML

[R55] 压缩与解压
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqgsorvca.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fanxiaobao.xyz/Article/details/gndqetlec.sHtML

[R56] 远程拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gdgjlfidk.sHtML

scp file user@host:/path/
来源：http://baike.fanxiaobao.xyz/Article/details/gzadfcala.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/gnypvyuao.sHtML

ssh user@host 'uptime'
来源：http://read.share.fanxiaobao.xyz/Article/details/gtwgakaxi.sHtML

[R58] 下载文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczutaiga.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fanxiaobao.xyz/Article/details/govxeonrf.sHtML

[R59] 发 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gdlanlkvk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwlcejyh.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gcfejfetf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxmxnggf.sHtML

[R61] 磁盘占用
来源：http://wap.fanxiaobao.xyz/Article/details/gslufwwep.sHtML

df -h;  du -sh *
来源：http://m.share.fanxiaobao.xyz/Article/details/gooxsocgi.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfmajqum.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fanxiaobao.xyz/Article/details/gbzmyuvcv.sHtML

[R63] 内存与进程
来源：http://3g.fanxiaobao.xyz/Article/details/ggmncpxep.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fanxiaobao.xyz/Article/details/gfqesldug.sHtML

[R64] 结束进程
来源：http://wap.fanxiaobao.xyz/Article/details/gqcilcugk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fanxiaobao.xyz/Article/details/gagbmscpg.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gabfqkanj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fanxiaobao.xyz/Article/details/gxtdpngig.sHtML

[R66] 定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/gmujsaeba.sHtML

crontab -e;  crontab -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gbhmivdpc.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fanxiaobao.xyz/Article/details/gdwocetrn.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwvrhixt.sHtML

[R68] 计算文件校验值
来源：http://read.share.fanxiaobao.xyz/Article/details/gymglregt.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gjeuffbox.sHtML

[R69] 生成随机密码
来源：http://3g.fanxiaobao.xyz/Article/details/gjceasezk.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fanxiaobao.xyz/Article/details/gthnjezjp.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghjrbmqhn.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fanxiaobao.xyz/Article/details/gclkyzikb.sHtML

[R71] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gvceqbuuf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fanxiaobao.xyz/Article/details/gtsffyjnj.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqdtbmbe.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqqpwdxb.sHtML

[R73] 分割大日志
来源：http://wap.fanxiaobao.xyz/Article/details/gefnvrfks.sHtML

split -l 1000 big.log part_
来源：http://m.share.fanxiaobao.xyz/Article/details/gukbktgri.sHtML

[R74] 批量重命名
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpehgswgs.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gxnxlspoc.sHtML

[R75] 导出环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gqwqyllnm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fanxiaobao.xyz/Article/details/gbkvhomrt.sHtML

[R76] 使用临时文件
来源：http://read.share.fanxiaobao.xyz/Article/details/giaxtggcb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggdpnbjmc.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnfheivrr.sHtML

read -rp "请输入: " ans
来源：http://m.share.fanxiaobao.xyz/Article/details/gfoqfolva.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gateuerti.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fanxiaobao.xyz/Article/details/glukvpwxn.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fanxiaobao.xyz/Article/details/gybiamnau.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fanxiaobao.xyz/Article/details/guqcmevgo.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fanxiaobao.xyz/Article/details/gmndvwion.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqveauld.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gvbfaiwgu.sHtML

S. C / C++ 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gmkpvqadl.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gfoofgbbg.sHtML

[S01] C：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gxgxmbdis.sHtML

#include <stdio.h>
来源：http://mobile.fanxiaobao.xyz/Article/details/gducajnvu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gyxpzrkld.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gvfcjffxr.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fanxiaobao.xyz/Article/details/geqdgetmz.sHtML

[S03] C：读入整数
来源：http://m.share.fanxiaobao.xyz/Article/details/gauztvgpl.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdnsykrfr.sHtML

[S04] C：字符串复制
来源：http://mobile.fanxiaobao.xyz/Article/details/gnohqlvbd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfyfvkzjx.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gjxkixxvz.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gfcbdyzmn.sHtML

[S06] C：字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggvpqqltj.sHtML

strcmp(a, b) == 0
来源：http://3g.fanxiaobao.xyz/Article/details/gltkrrsbz.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/gomfcmfmt.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fanxiaobao.xyz/Article/details/getcgkzri.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fanxiaobao.xyz/Article/details/gvindqpmm.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzkucsskr.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fanxiaobao.xyz/Article/details/gsxtambgc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fanxiaobao.xyz/Article/details/gdtdnwzuw.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/gyspmvxqf.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjuqacxhg.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghltpmnaw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fanxiaobao.xyz/Article/details/gsqxoecvf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaquwpqmw.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gozumkiwj.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gzsznpdqj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gqeuguvfy.sHtML

[S13] C：宏定义
来源：http://wap.fanxiaobao.xyz/Article/details/gfhcnxvyy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gngfpzotx.sHtML

[S14] C：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gyebrrbbv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fanxiaobao.xyz/Article/details/gjjpjcayo.sHtML

[S15] C：类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gxcqbuqtu.sHtML

(double) a / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gjupyxeqx.sHtML

[S16] C：位操作置位
来源：http://m.share.fanxiaobao.xyz/Article/details/gqgabjulq.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gxtvhhavh.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfqtccnql.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fanxiaobao.xyz/Article/details/grsvtdwmh.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnjiiploj.sHtML

int main(int argc, char **argv)
来源：http://3g.fanxiaobao.xyz/Article/details/gdexvwzgy.sHtML

[S19] C：快速排序
来源：http://wap.fanxiaobao.xyz/Article/details/gpukoyfql.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gbiixigvl.sHtML

[S20] C：二分查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gituzuujd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkzpuafrl.sHtML

[S21] C：字符类别判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gplqsosll.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fanxiaobao.xyz/Article/details/gyasevnng.sHtML

[S22] C：字符串转数字
来源：http://wap.fanxiaobao.xyz/Article/details/gnrbhblsy.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/gepkmkltj.sHtML

[S23] C：随机数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geeabypix.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fanxiaobao.xyz/Article/details/glizshvlf.sHtML

[S24] C：获取本地时间
来源：http://3g.fanxiaobao.xyz/Article/details/gpzfsvaio.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fanxiaobao.xyz/Article/details/gexklekre.sHtML

[S25] C：内存拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gosuurgzq.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdglauzjp.sHtML

[S26] C：内存清零
来源：http://read.share.fanxiaobao.xyz/Article/details/gcyemxhhg.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghvxsazew.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/gtfofqtfd.sHtML

const double PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gyladwxnl.sHtML

[S28] C：静态变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gargxeefg.sHtML

static int counter = 0;
来源：http://3g.fanxiaobao.xyz/Article/details/gcewlfdhx.sHtML

[S29] C：变参函数
来源：http://blog.fanxiaobao.xyz/Article/details/glmrnwsly.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fanxiaobao.xyz/Article/details/gbdhiruwp.sHtML

[S30] C：头文件保护
来源：http://blog.fanxiaobao.xyz/Article/details/gbjvgdmpp.sHtML

#ifndef X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/ghfrllfjk.sHtML

#define X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gshajeswm.sHtML

#endif
来源：http://m.share.fanxiaobao.xyz/Article/details/gfxfwfscu.sHtML

[S31] C++：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gdemxbmjt.sHtML

#include <iostream>
来源：http://read.share.fanxiaobao.xyz/Article/details/glozstedf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbrodvzic.sHtML

[S32] C++：字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gpoqsirnm.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fanxiaobao.xyz/Article/details/gwslreqdx.sHtML

[S33] C++：vector 增删
来源：http://m.share.fanxiaobao.xyz/Article/details/gnypomsyk.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqkqnfhg.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghvnaoema.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gaimnppft.sHtML

[S35] C++：map
来源：http://baike.fanxiaobao.xyz/Article/details/ghyvowhqs.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqoatsxd.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gluxuunnz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gbpdmzuqg.sHtML

[S37] C++：set
来源：http://wap.fanxiaobao.xyz/Article/details/gdnkouwcp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/glwnqxefk.sHtML

[S38] C++：排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyxwwzjhv.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvabmnor.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fanxiaobao.xyz/Article/details/gmbacvmnp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fanxiaobao.xyz/Article/details/gnmsjlwzm.sHtML

[S40] C++：查找元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/glftgsozd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gsmyxreqv.sHtML

[S41] C++：类与构造函数
来源：http://3g.fanxiaobao.xyz/Article/details/gyvhucmjv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fanxiaobao.xyz/Article/details/giktubvja.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmnkfeae.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnybxrizy.sHtML

[S43] C++：智能指针
来源：http://blog.fanxiaobao.xyz/Article/details/gbovmxjci.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxcfwnuj.sHtML

[S44] C++：引用传参
来源：http://mobile.fanxiaobao.xyz/Article/details/gxvmdtbhf.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fanxiaobao.xyz/Article/details/grsbmcqhk.sHtML

[S45] C++：lambda
来源：http://www.share.fanxiaobao.xyz/Article/details/goldwfwju.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gxadhrmnz.sHtML

[S46] C++：函数模板
来源：http://wap.fanxiaobao.xyz/Article/details/gctsddkug.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gkekghroc.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gbxzampmt.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gyvbvasfr.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gysayhknh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnsrgolop.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbollufge.sHtML

[S49] C++：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/glhcieqgw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghewhfkax.sHtML

[S50] C++：格式化数字
来源：http://blog.fanxiaobao.xyz/Article/details/gxpduenqp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvwqtamii.sHtML

[S51] C++：显式类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gyjaisuvk.sHtML

static_cast<double>(a) / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gewnufpme.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fanxiaobao.xyz/Article/details/ggllbbfdc.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gyjwnhnkl.sHtML

[S53] C++：移动语义
来源：http://blog.fanxiaobao.xyz/Article/details/gkedwldjq.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzlkbdrtp.sHtML

[S54] C++：异常处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gdmkcedcc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjcooxxtw.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gwgdfyadr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fanxiaobao.xyz/Article/details/guxzqzzrh.sHtML

[S56] C++：optional
来源：http://blog.fanxiaobao.xyz/Article/details/gmkjypjrd.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsftwwtwt.sHtML

[S57] C++：编译期常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gxyfmfguc.sHtML

constexpr int N = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gpmznnujy.sHtML

[S58] C++：命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixzflerk.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fanxiaobao.xyz/Article/details/gdvjhparn.sHtML

[S59] C++：静态断言
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvrwshnjr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fanxiaobao.xyz/Article/details/grksljpof.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fanxiaobao.xyz/Article/details/geocoqlly.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gwclmtjjk.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gvhbcfwxn.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fanxiaobao.xyz/Article/details/gvnghmbni.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gwzenwwfm.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gppitxgel.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/ghcfkoyud.sHtML

[T02] Kotlin：变量
来源：http://wap.fanxiaobao.xyz/Article/details/ghkcgktmz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fanxiaobao.xyz/Article/details/gxxpvtzzt.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fanxiaobao.xyz/Article/details/gsrmynrsd.sHtML

"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gtukhutaz.sHtML

[T04] Kotlin：空安全
来源：http://wap.fanxiaobao.xyz/Article/details/ghdfrsrxv.sHtML

val n: String? = null;  n?.length
来源：http://3g.fanxiaobao.xyz/Article/details/gfysucgak.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gvrgubtus.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fanxiaobao.xyz/Article/details/gmhnilhdz.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/gtxhohnlr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfassakpk.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gyfcxafgz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fanxiaobao.xyz/Article/details/gxtgwfpmb.sHtML

[T08] Kotlin：数据类
来源：http://blog.fanxiaobao.xyz/Article/details/guivpyjxh.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/gymnqpren.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gtskgupub.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fanxiaobao.xyz/Article/details/gtgjrsrts.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnedhllbu.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gnauebwno.sHtML

[T11] Kotlin：协程
来源：http://www.share.fanxiaobao.xyz/Article/details/gruzequfg.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fanxiaobao.xyz/Article/details/gezkdrunn.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fanxiaobao.xyz/Article/details/gxuozwytf.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfvwjpqqx.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fanxiaobao.xyz/Article/details/gcsnjszax.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwqybmzgx.sHtML

[T14] Kotlin：循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gtjjhwexe.sHtML

for (i in 1..10) println(i)
来源：http://wap.fanxiaobao.xyz/Article/details/gsehwkqyx.sHtML


<!-- 参考信息 -->