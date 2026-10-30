代发 wailian999

echo "${#s}"
来源：http://www.share.fehbvm.com/Article/details/gsuuhwenk.sHtML

[R22] 截取子串
来源：http://read.share.hesvh.cn/Article/details/gnftqbjfy.sHtML

echo "${s:0:5}"
来源：http://read.share.zdbjq.cn/Article/details/gvzrnbbka.sHtML

[R23] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/gbcczlgru.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.hesvh.cn/Article/details/gvovonnlc.sHtML

[R24] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/gnvwjrgbm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.hesvh.cn/Article/details/ggugqqzst.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.zdbjq.cn/Article/details/gciwnbyuc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.hesvh.cn/Article/details/gmpjkyruu.sHtML

[R26] 命令替换
来源：http://read.share.fehbvm.com/Article/details/gqzwwnezw.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.hesvh.cn/Article/details/getjticmj.sHtML

[R27] 算术展开
来源：http://www.share.zdbjq.cn/Article/details/gacjpiums.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.zdbjq.cn/Article/details/gzujpxgmm.sHtML

[R28] 浮点运算
来源：http://read.share.fehbvm.com/Article/details/gicuxornp.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fehbvm.com/Article/details/gqyukwibf.sHtML

[R29] 定义函数
来源：http://wap.fehbvm.com/Article/details/gkxxjifha.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.zdbjq.cn/Article/details/gyzcmoamc.sHtML

[R30] 函数返回状态码
来源：http://www.blog.zdbjq.cn/Article/details/gcaowabef.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.zdbjq.cn/Article/details/gijspfkmn.sHtML

[R31] 局部变量
来源：http://read.share.zdbjq.cn/Article/details/gyscmspkt.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.zdbjq.cn/Article/details/gbbjksmtc.sHtML

[R32] 参数个数校验
来源：http://mobile.hesvh.cn/Article/details/gsazivopl.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gergsakdc.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fehbvm.com/Article/details/gmziwvsah.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.hesvh.cn/Article/details/geylgjlni.sHtML

[R34] 退出时清理
来源：http://m.share.fehbvm.com/Article/details/gsbwngicx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/gpyikfyme.sHtML

[R35] 后台执行并等待
来源：http://www.share.fehbvm.com/Article/details/gwhszbadn.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.zdbjq.cn/Article/details/gaymbqqjb.sHtML

[R36] 并发执行多个任务
来源：http://wap.fehbvm.com/Article/details/gglwtphyf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.hesvh.cn/Article/details/gpfkakwxv.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fehbvm.com/Article/details/gmoxiqizs.sHtML

files=$(ls -1)
来源：http://baike.fehbvm.com/Article/details/grdszgmgk.sHtML

[R38] 管道串联
来源：http://www.share.hesvh.cn/Article/details/gqxzhbjrv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.zdbjq.cn/Article/details/gzdwqbfzl.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.hesvh.cn/Article/details/glefqvbae.sHtML

cmd > out.log 2>&1
来源：http://wap.zdbjq.cn/Article/details/gnhepcvvv.sHtML

[R40] 追加写日志
来源：http://3g.zdbjq.cn/Article/details/gfdppvcyo.sHtML

echo "log" >> out.log
来源：http://mobile.zdbjq.cn/Article/details/gqcrycmvs.sHtML

[R41] 丢弃输出
来源：http://blog.fehbvm.com/Article/details/gqgolupcs.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fehbvm.com/Article/details/gctiqfqlm.sHtML

[R42] 输入重定向
来源：http://www.m.share.fehbvm.com/Article/details/gfjrmrhgq.sHtML

wc -l < a.txt
来源：http://read.share.fehbvm.com/Article/details/gnqqcilbn.sHtML

[R43] 按名字查找文件
来源：http://blog.zdbjq.cn/Article/details/gxyqoleyp.sHtML

find . -name "*.log" -type f
来源：http://www.blog.hesvh.cn/Article/details/gxlmdfhxo.sHtML

[R44] 按修改时间查找
来源：http://3g.zdbjq.cn/Article/details/gdiwvhmhk.sHtML

find . -mtime -7 -type f
来源：http://m.share.fehbvm.com/Article/details/gxvfvkohe.sHtML

[R45] 批量删除
来源：http://www.blog.hesvh.cn/Article/details/giwmjsnum.sHtML

find . -name "*.tmp" -delete
来源：http://baike.zdbjq.cn/Article/details/gwrqoopnp.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.hesvh.cn/Article/details/gomsojwkl.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.hesvh.cn/Article/details/gzcabrxfu.sHtML

[R47] sed 单行替换
来源：http://blog.zdbjq.cn/Article/details/ghgsejaru.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.hesvh.cn/Article/details/gsqqvobxg.sHtML

[R48] awk 取指定列
来源：http://wap.fehbvm.com/Article/details/groelmpuz.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fehbvm.com/Article/details/ghoupfyzm.sHtML

[R49] awk 带条件
来源：http://blog.zdbjq.cn/Article/details/gychxulvg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fehbvm.com/Article/details/gsqqdsycv.sHtML

[R50] awk 求和
来源：http://www.blog.fehbvm.com/Article/details/gifbrmssj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fehbvm.com/Article/details/govhuvaag.sHtML

[R51] 排序去重取前几
来源：http://wap.fehbvm.com/Article/details/gszfaajgl.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.hesvh.cn/Article/details/gcjblhowv.sHtML

[R52] 统计行数
来源：http://blog.hesvh.cn/Article/details/gzslehwxd.sHtML

wc -l a.txt
来源：http://3g.fehbvm.com/Article/details/gzswsaeen.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.hesvh.cn/Article/details/goxrpvxfy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.zdbjq.cn/Article/details/gzckwyvgk.sHtML

[R54] 比较两个文件
来源：http://baike.fehbvm.com/Article/details/gthsxccdb.sHtML

diff a.txt b.txt
来源：http://mobile.zdbjq.cn/Article/details/gavmtqqce.sHtML

[R55] 压缩与解压
来源：http://www.m.share.hesvh.cn/Article/details/gpnvrzhex.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.zdbjq.cn/Article/details/gvhjtzvbg.sHtML

[R56] 远程拷贝
来源：http://mobile.hesvh.cn/Article/details/gwizaggny.sHtML

scp file user@host:/path/
来源：http://www.blog.fehbvm.com/Article/details/gilrlfeuw.sHtML

[R57] 远程执行命令
来源：http://baike.hesvh.cn/Article/details/gxxjlpjjb.sHtML

ssh user@host 'uptime'
来源：http://wap.fehbvm.com/Article/details/gmtasmndb.sHtML

[R58] 下载文件
来源：http://mobile.fehbvm.com/Article/details/gzrjlnxdd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fehbvm.com/Article/details/gazwfxtjf.sHtML

[R59] 发 POST JSON
来源：http://baike.fehbvm.com/Article/details/ghtbawdfk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.zdbjq.cn/Article/details/gwxatldtn.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.hesvh.cn/Article/details/gfdkcikpl.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fehbvm.com/Article/details/gnwjdimsq.sHtML

[R61] 磁盘占用
来源：http://blog.zdbjq.cn/Article/details/gspqbdemq.sHtML

df -h;  du -sh *
来源：http://www.share.hesvh.cn/Article/details/ghruisrgh.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.zdbjq.cn/Article/details/gjumketyx.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.hesvh.cn/Article/details/ggyfpbdkt.sHtML

[R63] 内存与进程
来源：http://www.blog.zdbjq.cn/Article/details/gbandstvc.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fehbvm.com/Article/details/gkrnekniq.sHtML

[R64] 结束进程
来源：http://www.blog.hesvh.cn/Article/details/gyaxeqidh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fehbvm.com/Article/details/gmbyzduow.sHtML

[R65] 查看端口占用
来源：http://mobile.zdbjq.cn/Article/details/gvnmwsjfi.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.zdbjq.cn/Article/details/glcpfxdho.sHtML

[R66] 定时任务
来源：http://baike.hesvh.cn/Article/details/gaiisfbfv.sHtML

crontab -e;  crontab -l
来源：http://read.share.hesvh.cn/Article/details/glwuwbfks.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.zdbjq.cn/Article/details/gploscdvd.sHtML

openssl rand -hex 16
来源：http://www.share.hesvh.cn/Article/details/gaciyazao.sHtML

[R68] 计算文件校验值
来源：http://read.share.fehbvm.com/Article/details/gcyyouuwl.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.zdbjq.cn/Article/details/ggzpjprwo.sHtML

[R69] 生成随机密码
来源：http://blog.fehbvm.com/Article/details/gvwzoeiph.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.hesvh.cn/Article/details/gcbcrqkgx.sHtML

[R70] 时间戳与互转
来源：http://baike.fehbvm.com/Article/details/gcipjskix.sHtML

date +%s;  date -d @1700000000
来源：http://wap.zdbjq.cn/Article/details/ghqyofrmw.sHtML

[R71] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/grihapgei.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fehbvm.com/Article/details/gbqufokhb.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fehbvm.com/Article/details/gzflwaufr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/grrtwobvz.sHtML

[R73] 分割大日志
来源：http://mobile.fehbvm.com/Article/details/ghxysvjqa.sHtML

split -l 1000 big.log part_
来源：http://wap.hesvh.cn/Article/details/ggetrkxus.sHtML

[R74] 批量重命名
来源：http://3g.zdbjq.cn/Article/details/gycjnnkwu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.hesvh.cn/Article/details/ggkgbtkbp.sHtML

[R75] 导出环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gfzlzzani.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fehbvm.com/Article/details/gguovtgpy.sHtML

[R76] 使用临时文件
来源：http://www.blog.zdbjq.cn/Article/details/gnddarepe.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/gmluvkudm.sHtML

[R77] 读取用户输入
来源：http://www.blog.zdbjq.cn/Article/details/gekcqwtvk.sHtML

read -rp "请输入: " ans
来源：http://wap.fehbvm.com/Article/details/gwuwyjygv.sHtML

[R78] 交互式菜单
来源：http://blog.hesvh.cn/Article/details/gcymgpqmt.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.hesvh.cn/Article/details/gxhdofakf.sHtML

[R79] 解析命令行选项
来源：http://blog.fehbvm.com/Article/details/gwdddwszh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.zdbjq.cn/Article/details/gjnlmifyh.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fehbvm.com/Article/details/glgvwvphj.sHtML

time ./run.sh
来源：http://m.share.hesvh.cn/Article/details/ghprfprtb.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/geywfemtk.sHtML

S. C / C++ 专题
来源：http://www.share.zdbjq.cn/Article/details/galrdwzbl.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gscjsvima.sHtML

[S01] C：Hello World
来源：http://baike.hesvh.cn/Article/details/guunxwiof.sHtML

#include <stdio.h>
来源：http://wap.fehbvm.com/Article/details/gibvktnmi.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.zdbjq.cn/Article/details/grcadtjvd.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.hesvh.cn/Article/details/ggsxxgwij.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.hesvh.cn/Article/details/gfmuishev.sHtML

[S03] C：读入整数
来源：http://blog.hesvh.cn/Article/details/gvwjpqqcs.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.zdbjq.cn/Article/details/gdznchakg.sHtML

[S04] C：字符串复制
来源：http://m.share.zdbjq.cn/Article/details/gybxjegmr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.zdbjq.cn/Article/details/gcslawykt.sHtML

[S05] C：字符串长度
来源：http://www.share.hesvh.cn/Article/details/gdxnumqgv.sHtML

strlen(s)
来源：http://www.m.share.fehbvm.com/Article/details/gukencdnq.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gqvmrndri.sHtML

strcmp(a, b) == 0
来源：http://mobile.fehbvm.com/Article/details/gdqbfgcqt.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fehbvm.com/Article/details/gcslroifr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fehbvm.com/Article/details/gqxkbbmxq.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.hesvh.cn/Article/details/glhbpiftm.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.zdbjq.cn/Article/details/gisxgvlsl.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.zdbjq.cn/Article/details/gilywxowt.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fehbvm.com/Article/details/gkwdvcnft.sHtML

[S10] C：指针与解引用
来源：http://wap.zdbjq.cn/Article/details/gocnkqlqq.sHtML

int *p = &a;  *p = 5;
来源：http://3g.zdbjq.cn/Article/details/gnuhnxbtt.sHtML

[S11] C：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gkbzuemmq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.hesvh.cn/Article/details/gjrzvrjgo.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.zdbjq.cn/Article/details/gabypbxgq.sHtML

fclose(f);
来源：http://3g.zdbjq.cn/Article/details/gvuzvxmis.sHtML

[S12] C：写文件
来源：http://mobile.zdbjq.cn/Article/details/gmcmijngg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.hesvh.cn/Article/details/guqmxaurh.sHtML

[S13] C：宏定义
来源：http://www.blog.zdbjq.cn/Article/details/gtzeeqroz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.hesvh.cn/Article/details/gpapmmkhr.sHtML

[S14] C：枚举
来源：http://wap.fehbvm.com/Article/details/gtktwyffc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.zdbjq.cn/Article/details/gsnfkdcdr.sHtML

[S15] C：类型转换
来源：http://wap.hesvh.cn/Article/details/gqwlwbmhc.sHtML

(double) a / b
来源：http://m.share.zdbjq.cn/Article/details/gzmmbbwia.sHtML

[S16] C：位操作置位
来源：http://mobile.zdbjq.cn/Article/details/gvebrprgf.sHtML

x |= (1 << 3);
来源：http://3g.hesvh.cn/Article/details/gsiehtuor.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gufkxlxvl.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.hesvh.cn/Article/details/gyvgqloan.sHtML

[S18] C：命令行参数
来源：http://www.blog.fehbvm.com/Article/details/gtkkzgvhx.sHtML

int main(int argc, char **argv)
来源：http://blog.zdbjq.cn/Article/details/giqmchukt.sHtML

[S19] C：快速排序
来源：http://wap.hesvh.cn/Article/details/gizrisolt.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gcruwhkva.sHtML

[S20] C：二分查找
来源：http://mobile.fehbvm.com/Article/details/gvrozgybj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/gfnfjajgg.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fehbvm.com/Article/details/gafkexdoc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fehbvm.com/Article/details/gdelomgkh.sHtML

[S22] C：字符串转数字
来源：http://read.share.zdbjq.cn/Article/details/gpdcvafco.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.hesvh.cn/Article/details/ggasigths.sHtML

[S23] C：随机数
来源：http://www.blog.hesvh.cn/Article/details/gltiurofb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.zdbjq.cn/Article/details/gghcvlkca.sHtML

[S24] C：获取本地时间
来源：http://www.share.zdbjq.cn/Article/details/gurtuhqut.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fehbvm.com/Article/details/gkrtpbsoe.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gjqkmuhoa.sHtML

memcpy(dst, src, n);
来源：http://wap.fehbvm.com/Article/details/gbxpggaix.sHtML

[S26] C：内存清零
来源：http://www.m.share.hesvh.cn/Article/details/guytofhqy.sHtML

memset(a, 0, sizeof a);
来源：http://3g.zdbjq.cn/Article/details/gzpftfatv.sHtML

[S27] C：定义常量
来源：http://www.blog.hesvh.cn/Article/details/gsrxpuwbz.sHtML

const double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/grbgmpnaf.sHtML

[S28] C：静态变量
来源：http://www.blog.fehbvm.com/Article/details/gphpfhkxr.sHtML

static int counter = 0;
来源：http://read.share.zdbjq.cn/Article/details/gqlfsxrnb.sHtML

[S29] C：变参函数
来源：http://read.share.fehbvm.com/Article/details/gvybotebk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.hesvh.cn/Article/details/gsirecjht.sHtML

[S30] C：头文件保护
来源：http://baike.zdbjq.cn/Article/details/gkhmawgyq.sHtML

#ifndef X_H
来源：http://www.share.zdbjq.cn/Article/details/gznqgsgzj.sHtML

#define X_H
来源：http://m.share.hesvh.cn/Article/details/gxvwrudgf.sHtML

#endif
来源：http://3g.zdbjq.cn/Article/details/gvthncodm.sHtML

[S31] C++：Hello World
来源：http://m.share.fehbvm.com/Article/details/gvnyvpbus.sHtML

#include <iostream>
来源：http://www.share.hesvh.cn/Article/details/gztpvnuch.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.hesvh.cn/Article/details/gjocxbqns.sHtML

[S32] C++：字符串
来源：http://baike.fehbvm.com/Article/details/gppzxhbfr.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.hesvh.cn/Article/details/gjkfgjdjy.sHtML

[S33] C++：vector 增删
来源：http://m.share.zdbjq.cn/Article/details/giyrrvvij.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gsudsmjtc.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.hesvh.cn/Article/details/gizanbewv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fehbvm.com/Article/details/gzosfaopc.sHtML

[S35] C++：map
来源：http://www.blog.hesvh.cn/Article/details/gbgqjtwkb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/guuapdwuk.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.zdbjq.cn/Article/details/gdqspkuql.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/gnueeenmz.sHtML

[S37] C++：set
来源：http://baike.zdbjq.cn/Article/details/gpcgxjtmr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.hesvh.cn/Article/details/gxecqtxly.sHtML

[S38] C++：排序
来源：http://blog.fehbvm.com/Article/details/gdsswkiox.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.hesvh.cn/Article/details/grikockia.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fehbvm.com/Article/details/gpfhrswai.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.hesvh.cn/Article/details/gpqlskayk.sHtML

[S40] C++：查找元素
来源：http://mobile.zdbjq.cn/Article/details/gnkkceydc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.hesvh.cn/Article/details/gjrfueekr.sHtML

[S41] C++：类与构造函数
来源：http://mobile.hesvh.cn/Article/details/gqqvrazab.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fehbvm.com/Article/details/gamytotje.sHtML

[S42] C++：继承与虚函数
来源：http://blog.hesvh.cn/Article/details/gyiphnhmh.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fehbvm.com/Article/details/gybatcozz.sHtML

[S43] C++：智能指针
来源：http://3g.hesvh.cn/Article/details/glgnrawmz.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.zdbjq.cn/Article/details/glbgynrbl.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fehbvm.com/Article/details/grfyhnnxc.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.hesvh.cn/Article/details/gxgszyqek.sHtML

[S45] C++：lambda
来源：http://baike.zdbjq.cn/Article/details/gvalvliwi.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.zdbjq.cn/Article/details/gilinetru.sHtML

[S46] C++：函数模板
来源：http://3g.zdbjq.cn/Article/details/gzqrtjgiv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.hesvh.cn/Article/details/gdtzvopui.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fehbvm.com/Article/details/gdlrwseat.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.zdbjq.cn/Article/details/gzyqwprwh.sHtML

[S48] C++：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gcoetvjsh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.hesvh.cn/Article/details/geoagzdvf.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.hesvh.cn/Article/details/glsqrwytg.sHtML

[S49] C++：写文件
来源：http://www.share.zdbjq.cn/Article/details/gfrcjhuek.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.zdbjq.cn/Article/details/ghstuifsn.sHtML

[S50] C++：格式化数字
来源：http://wap.zdbjq.cn/Article/details/guhwbyjda.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gzgohtqgh.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.hesvh.cn/Article/details/ghmhxnvco.sHtML

static_cast<double>(a) / b
来源：http://read.share.hesvh.cn/Article/details/gaowjbexg.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fehbvm.com/Article/details/gjulpqzxy.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.zdbjq.cn/Article/details/gwyewntsj.sHtML

[S53] C++：移动语义
来源：http://blog.zdbjq.cn/Article/details/gjlklhduy.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.zdbjq.cn/Article/details/gfcvvutrd.sHtML

[S54] C++：异常处理
来源：http://baike.hesvh.cn/Article/details/gxqlzrmjc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.zdbjq.cn/Article/details/gbttdekzw.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fehbvm.com/Article/details/gmjdrawof.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fehbvm.com/Article/details/gmlxhentf.sHtML

[S56] C++：optional
来源：http://mobile.zdbjq.cn/Article/details/guaoctsoz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.hesvh.cn/Article/details/gfnxitlai.sHtML

[S57] C++：编译期常量
来源：http://3g.fehbvm.com/Article/details/gxxpemloy.sHtML

constexpr int N = 10;
来源：http://mobile.fehbvm.com/Article/details/gqgprgghm.sHtML

[S58] C++：命名空间
来源：http://www.blog.zdbjq.cn/Article/details/gzhpelfov.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fehbvm.com/Article/details/gmvgdcrlb.sHtML

[S59] C++：静态断言
来源：http://wap.fehbvm.com/Article/details/gevuqwzuh.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.zdbjq.cn/Article/details/gjxeqcbsk.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fehbvm.com/Article/details/gbgphyxyk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gdptrvmsa.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gkzhyrjvc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.zdbjq.cn/Article/details/gnxktjkuu.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gicecmjzy.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fehbvm.com/Article/details/gsjxfwtij.sHtML

println("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gbycfeeuw.sHtML

[T02] Kotlin：变量
来源：http://www.blog.zdbjq.cn/Article/details/gwtgkkiig.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fehbvm.com/Article/details/ggqlaazkw.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.hesvh.cn/Article/details/gnvxybuzy.sHtML

"值: $b"
来源：http://m.share.fehbvm.com/Article/details/gqvuskjzb.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fehbvm.com/Article/details/gxbjitjhy.sHtML

val n: String? = null;  n?.length
来源：http://3g.hesvh.cn/Article/details/grmpcjowk.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.hesvh.cn/Article/details/gfwohcnhk.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fehbvm.com/Article/details/glzytsbjn.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.zdbjq.cn/Article/details/gijufgwsx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.zdbjq.cn/Article/details/gxxhhgkck.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/gefstppxb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.zdbjq.cn/Article/details/glgvannbc.sHtML

[T08] Kotlin：数据类
来源：http://blog.hesvh.cn/Article/details/gxvdbmvqb.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.zdbjq.cn/Article/details/gkkkocwzo.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.hesvh.cn/Article/details/ggbmlbmqq.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fehbvm.com/Article/details/gckxpocxu.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.hesvh.cn/Article/details/ggzushpjg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.hesvh.cn/Article/details/goxnskwpx.sHtML

[T11] Kotlin：协程
来源：http://baike.hesvh.cn/Article/details/gumzugqyc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.hesvh.cn/Article/details/gcwupwspt.sHtML

[T12] Kotlin：解构声明
来源：http://blog.zdbjq.cn/Article/details/gfyuddjol.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gwrbjwksm.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fehbvm.com/Article/details/gxamfblzg.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.hesvh.cn/Article/details/gigdunvoc.sHtML

[T14] Kotlin：循环
来源：http://wap.fehbvm.com/Article/details/guotywyia.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.hesvh.cn/Article/details/ggkjbkehb.sHtML

[T15] Kotlin：接口
来源：http://read.share.fehbvm.com/Article/details/gsalsyqgy.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fehbvm.com/Article/details/gvjmpizvk.sHtML

[T16] Swift：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gyfxehcyh.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/gxhxsvpdm.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fehbvm.com/Article/details/gjwnahndp.sHtML

var a = 1;  let b = 2
来源：http://3g.zdbjq.cn/Article/details/gogjahpem.sHtML

[T18] Swift：字符串插值
来源：http://3g.hesvh.cn/Article/details/gnmjwxebh.sHtML

"值: \(b)"
来源：http://wap.fehbvm.com/Article/details/gbxwflxgk.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fehbvm.com/Article/details/gcevemvqr.sHtML

if let n = opt { print(n) }
来源：http://blog.zdbjq.cn/Article/details/gfphafxmb.sHtML

[T20] Swift：数组操作
来源：http://read.share.zdbjq.cn/Article/details/glahjlwgm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.hesvh.cn/Article/details/gaaqiyoev.sHtML

[T21] Swift：遍历
来源：http://read.share.hesvh.cn/Article/details/gecwgcfqd.sHtML

for x in a { print(x) }
来源：http://read.share.hesvh.cn/Article/details/gjjwnvfhq.sHtML

[T22] Swift：字典
来源：http://baike.zdbjq.cn/Article/details/gubxaydtc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fehbvm.com/Article/details/ghycatxwk.sHtML

[T23] Swift：函数
来源：http://baike.hesvh.cn/Article/details/gzbrevpfg.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fehbvm.com/Article/details/ganexbljo.sHtML

[T24] Swift：闭包
来源：http://www.m.share.zdbjq.cn/Article/details/gcvfvtsmg.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.hesvh.cn/Article/details/gwrmcqjhg.sHtML


<!-- 参考信息 -->