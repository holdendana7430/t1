代发 wailian999

esac
来源：http://blog.zdbjq.cn/Article/details/gyxykazcm.sHtML

[R12] for 遍历文件
来源：http://baike.hesvh.cn/Article/details/gvmrkfkse.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fehbvm.com/Article/details/gnwfqbmim.sHtML

[R13] for 计数循环
来源：http://m.share.hesvh.cn/Article/details/gdwnnvksr.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fehbvm.com/Article/details/gdirnhxzs.sHtML

[R14] C 风格 for
来源：http://m.share.zdbjq.cn/Article/details/gawvkzwwv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/giramueog.sHtML

[R15] while 逐行读文件
来源：http://wap.hesvh.cn/Article/details/gkndyptxf.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.hesvh.cn/Article/details/gfygejdfu.sHtML

[R16] until 等待条件
来源：http://www.share.hesvh.cn/Article/details/gidmxrvai.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gpkxcxttv.sHtML

[R17] 数组定义与取值
来源：http://baike.hesvh.cn/Article/details/gidpxcphn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.hesvh.cn/Article/details/gzzbwitzy.sHtML

[R18] 遍历数组
来源：http://m.share.zdbjq.cn/Article/details/gemfqkwtz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gporadkyb.sHtML

[R19] 数组长度
来源：http://3g.hesvh.cn/Article/details/gviskfdgn.sHtML

echo "${#arr[@]}"
来源：http://3g.zdbjq.cn/Article/details/gudlvoesk.sHtML

[R20] 关联数组（字典）
来源：http://mobile.zdbjq.cn/Article/details/gwwmbmhzv.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.hesvh.cn/Article/details/gyucrkbyv.sHtML

[R21] 字符串长度
来源：http://wap.hesvh.cn/Article/details/gjzwyhvrf.sHtML

echo "${#s}"
来源：http://www.blog.hesvh.cn/Article/details/ghyesvykx.sHtML

[R22] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/gszmjzezf.sHtML

echo "${s:0:5}"
来源：http://www.share.zdbjq.cn/Article/details/guqnwdjod.sHtML

[R23] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/gektpmbhb.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.hesvh.cn/Article/details/gwhxncqto.sHtML

[R24] 大小写转换
来源：http://baike.hesvh.cn/Article/details/gtfsyajea.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fehbvm.com/Article/details/gfcitsffd.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fehbvm.com/Article/details/geuxgdtlu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.zdbjq.cn/Article/details/gldniayss.sHtML

[R26] 命令替换
来源：http://www.share.fehbvm.com/Article/details/gpdpcrmcs.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.zdbjq.cn/Article/details/gplmabeib.sHtML

[R27] 算术展开
来源：http://www.blog.hesvh.cn/Article/details/gcpkfpssr.sHtML

echo $((1 + 2 * 3))
来源：http://blog.zdbjq.cn/Article/details/gcwskppuu.sHtML

[R28] 浮点运算
来源：http://blog.hesvh.cn/Article/details/gkuevfspf.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.zdbjq.cn/Article/details/gxrssgmpf.sHtML

[R29] 定义函数
来源：http://www.share.fehbvm.com/Article/details/gtniiiekb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.zdbjq.cn/Article/details/ggodpeyub.sHtML

[R30] 函数返回状态码
来源：http://m.share.hesvh.cn/Article/details/gpspgrcpq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.zdbjq.cn/Article/details/garkrpkkk.sHtML

[R31] 局部变量
来源：http://www.blog.hesvh.cn/Article/details/gwaenxogv.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fehbvm.com/Article/details/gzyelyduw.sHtML

[R32] 参数个数校验
来源：http://www.m.share.hesvh.cn/Article/details/ggxniazye.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/glyevaerr.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.zdbjq.cn/Article/details/gwcwcopyw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.zdbjq.cn/Article/details/grrozzzad.sHtML

[R34] 退出时清理
来源：http://www.blog.zdbjq.cn/Article/details/ggvoxzzqf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.hesvh.cn/Article/details/gvsmjvuoz.sHtML

[R35] 后台执行并等待
来源：http://3g.fehbvm.com/Article/details/gsqcpuxlp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.hesvh.cn/Article/details/gdxrrrgha.sHtML

[R36] 并发执行多个任务
来源：http://www.share.hesvh.cn/Article/details/gmgegfqva.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.zdbjq.cn/Article/details/giphuksqf.sHtML

[R37] 把输出赋给变量
来源：http://wap.zdbjq.cn/Article/details/gffzcvejv.sHtML

files=$(ls -1)
来源：http://wap.hesvh.cn/Article/details/gbzmdbqyl.sHtML

[R38] 管道串联
来源：http://3g.hesvh.cn/Article/details/gshktrvcl.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.zdbjq.cn/Article/details/ggkvhvojp.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.zdbjq.cn/Article/details/gcstygswi.sHtML

cmd > out.log 2>&1
来源：http://wap.hesvh.cn/Article/details/gixpsruek.sHtML

[R40] 追加写日志
来源：http://3g.hesvh.cn/Article/details/gozslijus.sHtML

echo "log" >> out.log
来源：http://www.share.hesvh.cn/Article/details/gkolmihay.sHtML

[R41] 丢弃输出
来源：http://www.blog.fehbvm.com/Article/details/gmcsepeco.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fehbvm.com/Article/details/gfqsaacru.sHtML

[R42] 输入重定向
来源：http://wap.hesvh.cn/Article/details/gxrlslouv.sHtML

wc -l < a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gerpnfges.sHtML

[R43] 按名字查找文件
来源：http://3g.fehbvm.com/Article/details/gixpfqado.sHtML

find . -name "*.log" -type f
来源：http://blog.fehbvm.com/Article/details/ganfmbagz.sHtML

[R44] 按修改时间查找
来源：http://read.share.fehbvm.com/Article/details/gqystbfbn.sHtML

find . -mtime -7 -type f
来源：http://baike.hesvh.cn/Article/details/gcsciulyo.sHtML

[R45] 批量删除
来源：http://mobile.hesvh.cn/Article/details/grricqyng.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fehbvm.com/Article/details/gybjyvmfn.sHtML

[R46] 递归替换文件内容
来源：http://blog.fehbvm.com/Article/details/gosdsbgyx.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.zdbjq.cn/Article/details/gdukqebkq.sHtML

[R47] sed 单行替换
来源：http://www.share.fehbvm.com/Article/details/gemomvjsh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.hesvh.cn/Article/details/gtlnmmbjp.sHtML

[R48] awk 取指定列
来源：http://www.blog.fehbvm.com/Article/details/gtmvanqbz.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fehbvm.com/Article/details/goxshvtht.sHtML

[R49] awk 带条件
来源：http://3g.zdbjq.cn/Article/details/gnbphpdpq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.zdbjq.cn/Article/details/gjaxezvbk.sHtML

[R50] awk 求和
来源：http://m.share.zdbjq.cn/Article/details/guwusofed.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gprsvsezp.sHtML

[R51] 排序去重取前几
来源：http://read.share.fehbvm.com/Article/details/gyimtdxte.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.zdbjq.cn/Article/details/gevkkcwur.sHtML

[R52] 统计行数
来源：http://read.share.fehbvm.com/Article/details/gkwxntsau.sHtML

wc -l a.txt
来源：http://www.share.zdbjq.cn/Article/details/gstozcbxl.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fehbvm.com/Article/details/gylszolpu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.hesvh.cn/Article/details/gxxoareti.sHtML

[R54] 比较两个文件
来源：http://m.share.zdbjq.cn/Article/details/gqsiacmvf.sHtML

diff a.txt b.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gkxzwclab.sHtML

[R55] 压缩与解压
来源：http://www.share.fehbvm.com/Article/details/gtcnfyynm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.hesvh.cn/Article/details/gbfpkllan.sHtML

[R56] 远程拷贝
来源：http://3g.fehbvm.com/Article/details/gtddhxpzu.sHtML

scp file user@host:/path/
来源：http://www.share.hesvh.cn/Article/details/glpaabauw.sHtML

[R57] 远程执行命令
来源：http://wap.zdbjq.cn/Article/details/gjvzramas.sHtML

ssh user@host 'uptime'
来源：http://wap.fehbvm.com/Article/details/geojpslyt.sHtML

[R58] 下载文件
来源：http://m.share.zdbjq.cn/Article/details/gbqcsrmew.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.hesvh.cn/Article/details/gcvwvkdeh.sHtML

[R59] 发 POST JSON
来源：http://read.share.fehbvm.com/Article/details/gvfiycmtr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.zdbjq.cn/Article/details/gncqqsqlx.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/ggtcwdsbt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fehbvm.com/Article/details/ggosjmdld.sHtML

[R61] 磁盘占用
来源：http://mobile.zdbjq.cn/Article/details/gkpfplhgq.sHtML

df -h;  du -sh *
来源：http://www.share.fehbvm.com/Article/details/glrlmhthj.sHtML

[R62] 找最占空间的文件
来源：http://read.share.hesvh.cn/Article/details/gnkylckgi.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fehbvm.com/Article/details/gdnjgzwyd.sHtML

[R63] 内存与进程
来源：http://baike.hesvh.cn/Article/details/gvxvibtgf.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.zdbjq.cn/Article/details/gtflxkejp.sHtML

[R64] 结束进程
来源：http://blog.fehbvm.com/Article/details/gxggypimb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.hesvh.cn/Article/details/goplsfamg.sHtML

[R65] 查看端口占用
来源：http://www.share.fehbvm.com/Article/details/gijjwqjme.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fehbvm.com/Article/details/gsovquzzv.sHtML

[R66] 定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/ghiriybba.sHtML

crontab -e;  crontab -l
来源：http://blog.hesvh.cn/Article/details/ghqfgvcdr.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.hesvh.cn/Article/details/gmcprzjiy.sHtML

openssl rand -hex 16
来源：http://mobile.zdbjq.cn/Article/details/ggondrzvp.sHtML

[R68] 计算文件校验值
来源：http://www.blog.zdbjq.cn/Article/details/grjhaifva.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.hesvh.cn/Article/details/gwtgchvkq.sHtML

[R69] 生成随机密码
来源：http://3g.fehbvm.com/Article/details/grkkqqmwo.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fehbvm.com/Article/details/gpxaldazi.sHtML

[R70] 时间戳与互转
来源：http://blog.hesvh.cn/Article/details/gbootuyrg.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fehbvm.com/Article/details/grtjjoizj.sHtML

[R71] 日期格式化
来源：http://wap.fehbvm.com/Article/details/gkgrpxjal.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.hesvh.cn/Article/details/gjxwlwdjw.sHtML

[R72] 等待端口就绪
来源：http://www.share.fehbvm.com/Article/details/gxmapauyy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gprvdaafc.sHtML

[R73] 分割大日志
来源：http://3g.hesvh.cn/Article/details/gzyqjnedy.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.zdbjq.cn/Article/details/gkrcdfxin.sHtML

[R74] 批量重命名
来源：http://mobile.hesvh.cn/Article/details/gmedwyojs.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fehbvm.com/Article/details/gblyvcxxa.sHtML

[R75] 导出环境变量
来源：http://m.share.zdbjq.cn/Article/details/gilvqcudi.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.zdbjq.cn/Article/details/gozvlbwao.sHtML

[R76] 使用临时文件
来源：http://3g.hesvh.cn/Article/details/glezzmtgk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/gwqpnedqi.sHtML

[R77] 读取用户输入
来源：http://www.m.share.zdbjq.cn/Article/details/grpozkbmx.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.hesvh.cn/Article/details/guueqewlx.sHtML

[R78] 交互式菜单
来源：http://www.share.hesvh.cn/Article/details/gbfvxwlxs.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fehbvm.com/Article/details/gftxjhfpy.sHtML

[R79] 解析命令行选项
来源：http://baike.zdbjq.cn/Article/details/gyclonqlt.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.hesvh.cn/Article/details/gxisyqezf.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.zdbjq.cn/Article/details/gygcjtnik.sHtML

time ./run.sh
来源：http://mobile.zdbjq.cn/Article/details/gtigkvnzn.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/giowsphyj.sHtML

S. C / C++ 专题
来源：http://baike.hesvh.cn/Article/details/gbfkfuyvn.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gsibnhyjw.sHtML

[S01] C：Hello World
来源：http://blog.fehbvm.com/Article/details/gpjmhobvi.sHtML

#include <stdio.h>
来源：http://mobile.zdbjq.cn/Article/details/gdyzetybv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fehbvm.com/Article/details/gesbniqas.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fehbvm.com/Article/details/ghbtqykvk.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.hesvh.cn/Article/details/gtefmxbkn.sHtML

[S03] C：读入整数
来源：http://www.blog.hesvh.cn/Article/details/goyiovzkh.sHtML

int x; scanf("%d", &x);
来源：http://www.share.hesvh.cn/Article/details/gprimzphu.sHtML

[S04] C：字符串复制
来源：http://baike.zdbjq.cn/Article/details/gvavfvdba.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fehbvm.com/Article/details/gvxkhfgsb.sHtML

[S05] C：字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/grnpimdkm.sHtML

strlen(s)
来源：http://www.m.share.hesvh.cn/Article/details/gqrwviucj.sHtML

[S06] C：字符串比较
来源：http://wap.hesvh.cn/Article/details/ghytpjgbu.sHtML

strcmp(a, b) == 0
来源：http://m.share.fehbvm.com/Article/details/gjtklnqgw.sHtML

[S07] C：数组遍历求和
来源：http://blog.zdbjq.cn/Article/details/gumzbqwvt.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fehbvm.com/Article/details/gmzknfzui.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.zdbjq.cn/Article/details/gfxlhhmsz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.hesvh.cn/Article/details/gheopipny.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fehbvm.com/Article/details/gqmawpbgn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fehbvm.com/Article/details/gqwheubjc.sHtML

[S10] C：指针与解引用
来源：http://3g.fehbvm.com/Article/details/gvuawnthx.sHtML

int *p = &a;  *p = 5;
来源：http://blog.zdbjq.cn/Article/details/gyjpvdvrj.sHtML

[S11] C：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/golsknkts.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.zdbjq.cn/Article/details/gcqmqvtwm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.zdbjq.cn/Article/details/gzlvqmvkg.sHtML

fclose(f);
来源：http://3g.hesvh.cn/Article/details/gdbusysfz.sHtML

[S12] C：写文件
来源：http://baike.fehbvm.com/Article/details/gqtmretym.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/gqxlzzsvh.sHtML

[S13] C：宏定义
来源：http://baike.hesvh.cn/Article/details/gwggzrdwj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.hesvh.cn/Article/details/gawacpyeq.sHtML

[S14] C：枚举
来源：http://read.share.fehbvm.com/Article/details/gynexnflj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.hesvh.cn/Article/details/grthopyun.sHtML

[S15] C：类型转换
来源：http://read.share.hesvh.cn/Article/details/gzdjknmhf.sHtML

(double) a / b
来源：http://wap.fehbvm.com/Article/details/gxkuqxqwy.sHtML

[S16] C：位操作置位
来源：http://www.share.fehbvm.com/Article/details/gzbwjuptf.sHtML

x |= (1 << 3);
来源：http://m.share.zdbjq.cn/Article/details/gjrftcmvy.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gwnckqdgu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fehbvm.com/Article/details/gjfmhtwyb.sHtML

[S18] C：命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gggzhljtw.sHtML

int main(int argc, char **argv)
来源：http://read.share.hesvh.cn/Article/details/gqbfnieoj.sHtML

[S19] C：快速排序
来源：http://read.share.zdbjq.cn/Article/details/gkgoikagk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/gbdcbznue.sHtML

[S20] C：二分查找
来源：http://read.share.zdbjq.cn/Article/details/grwdegjji.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/gwfoqwndj.sHtML

[S21] C：字符类别判断
来源：http://mobile.hesvh.cn/Article/details/gzqiygbux.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.hesvh.cn/Article/details/gwowujimv.sHtML

[S22] C：字符串转数字
来源：http://blog.hesvh.cn/Article/details/glhluhjmx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.hesvh.cn/Article/details/ggmimxicw.sHtML

[S23] C：随机数
来源：http://read.share.fehbvm.com/Article/details/gfpqsglth.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.hesvh.cn/Article/details/gdrgxdaem.sHtML

[S24] C：获取本地时间
来源：http://read.share.fehbvm.com/Article/details/geycwilzp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.hesvh.cn/Article/details/gmbampptq.sHtML

[S25] C：内存拷贝
来源：http://3g.zdbjq.cn/Article/details/gipzpekmt.sHtML

memcpy(dst, src, n);
来源：http://blog.zdbjq.cn/Article/details/gbnpykkfp.sHtML

[S26] C：内存清零
来源：http://www.m.share.hesvh.cn/Article/details/gffdjgsxn.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.zdbjq.cn/Article/details/gmkccgmzs.sHtML

[S27] C：定义常量
来源：http://www.blog.hesvh.cn/Article/details/gcjfnrfph.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/ggxnmsfpg.sHtML

[S28] C：静态变量
来源：http://www.m.share.fehbvm.com/Article/details/gzipyovyo.sHtML

static int counter = 0;
来源：http://wap.fehbvm.com/Article/details/gqexouzsp.sHtML

[S29] C：变参函数
来源：http://m.share.hesvh.cn/Article/details/gnmrkcjdd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.zdbjq.cn/Article/details/gegahvkth.sHtML

[S30] C：头文件保护
来源：http://blog.fehbvm.com/Article/details/gddxyxabf.sHtML

#ifndef X_H
来源：http://3g.zdbjq.cn/Article/details/gmjbvgupd.sHtML

#define X_H
来源：http://read.share.zdbjq.cn/Article/details/gqaooobnt.sHtML

#endif
来源：http://mobile.fehbvm.com/Article/details/gwhhudrao.sHtML

[S31] C++：Hello World
来源：http://blog.zdbjq.cn/Article/details/gaxjnrxgl.sHtML

#include <iostream>
来源：http://blog.zdbjq.cn/Article/details/glagffsaa.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.hesvh.cn/Article/details/ghlglpfnl.sHtML

[S32] C++：字符串
来源：http://www.share.zdbjq.cn/Article/details/gxospfoes.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.zdbjq.cn/Article/details/ghfexdzdl.sHtML

[S33] C++：vector 增删
来源：http://blog.zdbjq.cn/Article/details/gcsshobku.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.hesvh.cn/Article/details/gyydquutg.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fehbvm.com/Article/details/gsqxrjlmr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fehbvm.com/Article/details/grtmebmad.sHtML

[S35] C++：map
来源：http://www.share.fehbvm.com/Article/details/gajyxpodd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/gsyhoasgt.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.hesvh.cn/Article/details/gbxnzrfoh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/gildynpue.sHtML

[S37] C++：set
来源：http://mobile.fehbvm.com/Article/details/gokewqcet.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fehbvm.com/Article/details/ggxsnudtt.sHtML

[S38] C++：排序
来源：http://www.share.zdbjq.cn/Article/details/gmbaxfxho.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.hesvh.cn/Article/details/gaztkmjtf.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.zdbjq.cn/Article/details/grvgfrndz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.zdbjq.cn/Article/details/gpmxfhzgb.sHtML

[S40] C++：查找元素
来源：http://3g.zdbjq.cn/Article/details/giucazoep.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.hesvh.cn/Article/details/gormttrim.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fehbvm.com/Article/details/gxdhnnhyc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fehbvm.com/Article/details/gajbcenaq.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.zdbjq.cn/Article/details/gywmysalq.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.hesvh.cn/Article/details/gkrbnsamm.sHtML

[S43] C++：智能指针
来源：http://mobile.hesvh.cn/Article/details/gecksqhmh.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.zdbjq.cn/Article/details/gxjdvueky.sHtML

[S44] C++：引用传参
来源：http://baike.hesvh.cn/Article/details/gnqnxuenv.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fehbvm.com/Article/details/gznnlgrtr.sHtML

[S45] C++：lambda
来源：http://wap.hesvh.cn/Article/details/gapuxmujd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fehbvm.com/Article/details/ggqsbfuxf.sHtML

[S46] C++：函数模板
来源：http://m.share.zdbjq.cn/Article/details/gxbmfsqqq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.hesvh.cn/Article/details/gheggljgu.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fehbvm.com/Article/details/gkwtrswyy.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.hesvh.cn/Article/details/gobemfclw.sHtML

[S48] C++：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gqkriupbo.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fehbvm.com/Article/details/gvlgwwhbl.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.hesvh.cn/Article/details/gzejiyrza.sHtML

[S49] C++：写文件
来源：http://read.share.zdbjq.cn/Article/details/gapgtqlgp.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.zdbjq.cn/Article/details/gmsbtyhvd.sHtML

[S50] C++：格式化数字
来源：http://baike.fehbvm.com/Article/details/gtseminnf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gbtkpafeo.sHtML

[S51] C++：显式类型转换
来源：http://blog.fehbvm.com/Article/details/gmafrbdun.sHtML

static_cast<double>(a) / b
来源：http://mobile.zdbjq.cn/Article/details/ggxnqpttv.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fehbvm.com/Article/details/glbhkgynf.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fehbvm.com/Article/details/gmaubschs.sHtML

[S53] C++：移动语义
来源：http://m.share.fehbvm.com/Article/details/guwzdtrjq.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fehbvm.com/Article/details/gyqmifyhr.sHtML

[S54] C++：异常处理
来源：http://baike.fehbvm.com/Article/details/gwpszshky.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gdbtsnlwv.sHtML

[S55] C++：结构化绑定
来源：http://baike.hesvh.cn/Article/details/gealwppbi.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.hesvh.cn/Article/details/gnbxqqaqx.sHtML

[S56] C++：optional
来源：http://read.share.zdbjq.cn/Article/details/gjlftfphk.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fehbvm.com/Article/details/gihbipsgv.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.hesvh.cn/Article/details/ggdqmywni.sHtML

constexpr int N = 10;
来源：http://3g.zdbjq.cn/Article/details/gwkggkojm.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fehbvm.com/Article/details/ghpqbybzr.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.hesvh.cn/Article/details/gnjjtqejo.sHtML

[S59] C++：静态断言
来源：http://www.blog.hesvh.cn/Article/details/gkvxvmqza.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.hesvh.cn/Article/details/gzhnvmibp.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.hesvh.cn/Article/details/grtbhjjzp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.hesvh.cn/Article/details/gkzuisxgm.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gegqpmhdr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.hesvh.cn/Article/details/gbcfgojcu.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gwzscgsxj.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gxkgzucwe.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/glryzbvpg.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.zdbjq.cn/Article/details/gbzastufl.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.hesvh.cn/Article/details/gnxgcgprt.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fehbvm.com/Article/details/gtvfkaeck.sHtML

"值: $b"
来源：http://3g.zdbjq.cn/Article/details/gcxreeikv.sHtML

[T04] Kotlin：空安全
来源：http://baike.zdbjq.cn/Article/details/gasujxqeg.sHtML

val n: String? = null;  n?.length
来源：http://blog.hesvh.cn/Article/details/gnkxhzjgy.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fehbvm.com/Article/details/gmgichrdk.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.hesvh.cn/Article/details/gwiojmtuz.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fehbvm.com/Article/details/gabkuupkh.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gkhvvshuw.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.zdbjq.cn/Article/details/galqtbjet.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.hesvh.cn/Article/details/ghfaaojio.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.zdbjq.cn/Article/details/ghwrbbjfj.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/gnanmuevj.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.hesvh.cn/Article/details/gezvhpzuf.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.zdbjq.cn/Article/details/gtmtzblzm.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.zdbjq.cn/Article/details/gzaqmnwqh.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.zdbjq.cn/Article/details/gaggfrvep.sHtML

[T11] Kotlin：协程
来源：http://baike.fehbvm.com/Article/details/gwpufijwo.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.hesvh.cn/Article/details/gyxtkjqih.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fehbvm.com/Article/details/gnzyapuvb.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fehbvm.com/Article/details/guodftsuc.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.zdbjq.cn/Article/details/grdzsbulb.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fehbvm.com/Article/details/gidoygnno.sHtML

[T14] Kotlin：循环
来源：http://wap.hesvh.cn/Article/details/gaqhxonuq.sHtML

for (i in 1..10) println(i)
来源：http://read.share.zdbjq.cn/Article/details/gjuttufam.sHtML


<!-- 参考信息 -->