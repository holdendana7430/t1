代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkhfxxsor.sHtML

[R26] 命令替换
来源：http://baike.fanxiaobao.xyz/Article/details/gzuhgrirz.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fanxiaobao.xyz/Article/details/gqawabgjl.sHtML

[R27] 算术展开
来源：http://mobile.fanxiaobao.xyz/Article/details/gilevclbx.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwhnhbqx.sHtML

[R28] 浮点运算
来源：http://3g.fanxiaobao.xyz/Article/details/gznmelavi.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fanxiaobao.xyz/Article/details/gxngxchwm.sHtML

[R29] 定义函数
来源：http://blog.fanxiaobao.xyz/Article/details/gvevkkzrd.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fanxiaobao.xyz/Article/details/ggclhhtbn.sHtML

[R30] 函数返回状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gmestpwre.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fanxiaobao.xyz/Article/details/gcwobzhun.sHtML

[R31] 局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwxvrshl.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpzooibtb.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guokfkldw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnclrbhqi.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fanxiaobao.xyz/Article/details/gcnvqnzlp.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fanxiaobao.xyz/Article/details/gksyiaeva.sHtML

[R34] 退出时清理
来源：http://m.share.fanxiaobao.xyz/Article/details/gwrrsatag.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gzpycrvvv.sHtML

[R35] 后台执行并等待
来源：http://blog.fanxiaobao.xyz/Article/details/gmanpfevx.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtkgbxynq.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwtviseke.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fanxiaobao.xyz/Article/details/gngzwnqqq.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gsojuaavm.sHtML

files=$(ls -1)
来源：http://wap.fanxiaobao.xyz/Article/details/ggrcieizt.sHtML

[R38] 管道串联
来源：http://blog.fanxiaobao.xyz/Article/details/gjtwtqogz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fanxiaobao.xyz/Article/details/grdsdagjc.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fanxiaobao.xyz/Article/details/ggjwfblhm.sHtML

cmd > out.log 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gmlalojgn.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnofuhdsg.sHtML

echo "log" >> out.log
来源：http://wap.fanxiaobao.xyz/Article/details/gkrwahpxp.sHtML

[R41] 丢弃输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gphlhxgqq.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gugeiqycs.sHtML

[R42] 输入重定向
来源：http://www.share.fanxiaobao.xyz/Article/details/gmnhzurcg.sHtML

wc -l < a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gzdnatkxu.sHtML

[R43] 按名字查找文件
来源：http://blog.fanxiaobao.xyz/Article/details/gyytarklh.sHtML

find . -name "*.log" -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gjhnakkhu.sHtML

[R44] 按修改时间查找
来源：http://3g.fanxiaobao.xyz/Article/details/ggnmymxpy.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gxphwcrpg.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/gkmipxlzy.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fanxiaobao.xyz/Article/details/gpklhvefw.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmbvmpbgu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtlwbmrav.sHtML

[R47] sed 单行替换
来源：http://www.share.fanxiaobao.xyz/Article/details/girbxqdrh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/goyifibwj.sHtML

[R48] awk 取指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/gqpvzpbwb.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gkgnhclve.sHtML

[R49] awk 带条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gzppkaafv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fanxiaobao.xyz/Article/details/gjnkwdlya.sHtML

[R50] awk 求和
来源：http://wap.fanxiaobao.xyz/Article/details/gbqmfszzy.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/grugqyilh.sHtML

[R51] 排序去重取前几
来源：http://baike.fanxiaobao.xyz/Article/details/gtmgohbsb.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaekjjsyk.sHtML

[R52] 统计行数
来源：http://read.share.fanxiaobao.xyz/Article/details/guauxfcei.sHtML

wc -l a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/giszidcdt.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fanxiaobao.xyz/Article/details/goxmhmsdc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgtajinl.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghhsfluuz.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gqgaeymeo.sHtML

[R55] 压缩与解压
来源：http://blog.fanxiaobao.xyz/Article/details/gunzemguf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fanxiaobao.xyz/Article/details/giuqmpvgm.sHtML

[R56] 远程拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gtxxsiqug.sHtML

scp file user@host:/path/
来源：http://baike.fanxiaobao.xyz/Article/details/gtxisvyrx.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gacfgrvsh.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjoyysfp.sHtML

[R58] 下载文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gggibjtsv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fanxiaobao.xyz/Article/details/gpdcxnfpk.sHtML

[R59] 发 POST JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/ghjpdmyqk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmywnxie.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gsbgxqcuc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfuvzkev.sHtML

[R61] 磁盘占用
来源：http://3g.fanxiaobao.xyz/Article/details/gesbtwhaw.sHtML

df -h;  du -sh *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gucwhuxxz.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzunhfhhr.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/gqjgehzgi.sHtML

[R63] 内存与进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gicysmgcx.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fanxiaobao.xyz/Article/details/gkzckurmj.sHtML

[R64] 结束进程
来源：http://www.share.fanxiaobao.xyz/Article/details/ggenjaugv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fanxiaobao.xyz/Article/details/ggdnlvcju.sHtML

[R65] 查看端口占用
来源：http://baike.fanxiaobao.xyz/Article/details/gcyjsxoxk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fanxiaobao.xyz/Article/details/gxlwcqebo.sHtML

[R66] 定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gpufsjaex.sHtML

crontab -e;  crontab -l
来源：http://baike.fanxiaobao.xyz/Article/details/gztwuwjat.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fanxiaobao.xyz/Article/details/gelhjavep.sHtML

openssl rand -hex 16
来源：http://baike.fanxiaobao.xyz/Article/details/gnytdiwqt.sHtML

[R68] 计算文件校验值
来源：http://baike.fanxiaobao.xyz/Article/details/glxlmwofq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnzlmbjyj.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/gpjfqxpwh.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fanxiaobao.xyz/Article/details/gcuainjsi.sHtML

[R70] 时间戳与互转
来源：http://wap.fanxiaobao.xyz/Article/details/gyslbrloy.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/gdeubwdpx.sHtML

[R71] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/ggopwuliu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fanxiaobao.xyz/Article/details/gnigwrcks.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/gmyvcjkcj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gbictriml.sHtML

[R73] 分割大日志
来源：http://baike.fanxiaobao.xyz/Article/details/gonyzeykm.sHtML

split -l 1000 big.log part_
来源：http://read.share.fanxiaobao.xyz/Article/details/gepedvrsn.sHtML

[R74] 批量重命名
来源：http://read.share.fanxiaobao.xyz/Article/details/gjaomravs.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gjmrphfar.sHtML

[R75] 导出环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/ggqhplqgs.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fanxiaobao.xyz/Article/details/gbvuomzml.sHtML

[R76] 使用临时文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gduvhvsyd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmmvkpug.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjhpvaso.sHtML

read -rp "请输入: " ans
来源：http://baike.fanxiaobao.xyz/Article/details/ghydbxvrc.sHtML

[R78] 交互式菜单
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjgaaybc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fanxiaobao.xyz/Article/details/gxmbeblck.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtnqtrqbp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fanxiaobao.xyz/Article/details/gsdldrhwq.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/gtdgiungu.sHtML

time ./run.sh
来源：http://3g.fanxiaobao.xyz/Article/details/gvtstpzvk.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gjecinutl.sHtML

S. C / C++ 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gepaappko.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gwuagwmsf.sHtML

[S01] C：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gkktulxnp.sHtML

#include <stdio.h>
来源：http://3g.fanxiaobao.xyz/Article/details/ggoenptwr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqhhryhcg.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbrqroiyu.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtdbliiqu.sHtML

[S03] C：读入整数
来源：http://baike.fanxiaobao.xyz/Article/details/ggegijzaq.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghyxqisps.sHtML

[S04] C：字符串复制
来源：http://3g.fanxiaobao.xyz/Article/details/gzuvueswi.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcummlxin.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/guamqhwfx.sHtML

strlen(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdvlcerhv.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwkkqzks.sHtML

strcmp(a, b) == 0
来源：http://blog.fanxiaobao.xyz/Article/details/gvrlacooi.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/gwtzzfjis.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/gcayounbd.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fanxiaobao.xyz/Article/details/gqrovqxev.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwntypoch.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fanxiaobao.xyz/Article/details/ghladuenw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fanxiaobao.xyz/Article/details/gnbhtzlqh.sHtML

[S10] C：指针与解引用
来源：http://blog.fanxiaobao.xyz/Article/details/gfdmyqqcs.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtkbsdqzs.sHtML

[S11] C：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gdpsbzhht.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/grvpqzpsa.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/giultryzp.sHtML

fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gchdjhymk.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gghoyrync.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbgcbxkty.sHtML

[S13] C：宏定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gxatqkwvx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fanxiaobao.xyz/Article/details/gibqujkek.sHtML

[S14] C：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfxfqthru.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fanxiaobao.xyz/Article/details/gdcqdmuzr.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gzoyshwaq.sHtML

(double) a / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gjdzrxlxj.sHtML

[S16] C：位操作置位
来源：http://blog.fanxiaobao.xyz/Article/details/gvrgaoowb.sHtML

x |= (1 << 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcrdzlctv.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gfhbmhyrx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fanxiaobao.xyz/Article/details/gcgysxldx.sHtML

[S18] C：命令行参数
来源：http://baike.fanxiaobao.xyz/Article/details/gxvjimnre.sHtML

int main(int argc, char **argv)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmmidgss.sHtML

[S19] C：快速排序
来源：http://wap.fanxiaobao.xyz/Article/details/gkueglhrv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghnlcxomr.sHtML

[S20] C：二分查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkzvesap.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gfsjhqpkq.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gffplfnlh.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwgfsjheo.sHtML

[S22] C：字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gxkqlkjpn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fanxiaobao.xyz/Article/details/gbkpandjx.sHtML

[S23] C：随机数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfdgsqtlf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gfkuqhqki.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/gldpaxcuf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fanxiaobao.xyz/Article/details/glbvthion.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gcsknttag.sHtML

memcpy(dst, src, n);
来源：http://baike.fanxiaobao.xyz/Article/details/ggaxlrgfp.sHtML

[S26] C：内存清零
来源：http://baike.fanxiaobao.xyz/Article/details/glyhqzdmk.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fanxiaobao.xyz/Article/details/gwuilkuxt.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/goznqpdls.sHtML

const double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gwzwhifky.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/ggrbfbifw.sHtML

static int counter = 0;
来源：http://wap.fanxiaobao.xyz/Article/details/gzghhfeny.sHtML

[S29] C：变参函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gkcwncwuh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghwdxkhy.sHtML

[S30] C：头文件保护
来源：http://m.share.fanxiaobao.xyz/Article/details/gxtiqzgns.sHtML

#ifndef X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grberfael.sHtML

#define X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/goqozbdgh.sHtML

#endif
来源：http://blog.fanxiaobao.xyz/Article/details/gqpzniyga.sHtML

[S31] C++：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/getakewzh.sHtML

#include <iostream>
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvymiiwf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gycbilzvq.sHtML

[S32] C++：字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gpsioiujb.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmlcuezws.sHtML

[S33] C++：vector 增删
来源：http://3g.fanxiaobao.xyz/Article/details/gpljrleeu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gwsryrfau.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvekxmvrt.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fanxiaobao.xyz/Article/details/ggvdjqecd.sHtML

[S35] C++：map
来源：http://baike.fanxiaobao.xyz/Article/details/gjulcglah.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gohdqhwnp.sHtML

[S36] C++：unordered_map
来源：http://www.share.fanxiaobao.xyz/Article/details/ghilxjmwl.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gnftxmktj.sHtML

[S37] C++：set
来源：http://www.share.fanxiaobao.xyz/Article/details/gnnzvjcwo.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gafogeisd.sHtML

[S38] C++：排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpvjiqxae.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gnhxpwvtr.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxzxohnz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fanxiaobao.xyz/Article/details/gitqlkcml.sHtML

[S40] C++：查找元素
来源：http://read.share.fanxiaobao.xyz/Article/details/glzkusrbx.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvcmcvaik.sHtML

[S41] C++：类与构造函数
来源：http://baike.fanxiaobao.xyz/Article/details/gcveqcwnv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gczbzmzhd.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fanxiaobao.xyz/Article/details/glijztbxy.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fanxiaobao.xyz/Article/details/gcpsylsub.sHtML

[S43] C++：智能指针
来源：http://m.share.fanxiaobao.xyz/Article/details/gcuxathkc.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghxpkznsn.sHtML

[S44] C++：引用传参
来源：http://mobile.fanxiaobao.xyz/Article/details/gdrdjtgvt.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gszlwizkc.sHtML

[S45] C++：lambda
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkfqtjnrw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwdpcoigw.sHtML

[S46] C++：函数模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/guwrqwsmu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpkvpbvds.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gvchspttx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gifwagohv.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrldjhcu.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fanxiaobao.xyz/Article/details/gofblrbyg.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gluisjskn.sHtML

[S49] C++：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gbvfnzegr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/gmdnhufkr.sHtML

[S50] C++：格式化数字
来源：http://blog.fanxiaobao.xyz/Article/details/gxkqvwmul.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnhlalcxk.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/girloigtp.sHtML

static_cast<double>(a) / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gszphwifv.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fanxiaobao.xyz/Article/details/gcydiayji.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmyiuqjlb.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwvjwburi.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkolxfbot.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsginydpf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxisbmnso.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/galyptkgw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwufeohzo.sHtML

[S56] C++：optional
来源：http://read.share.fanxiaobao.xyz/Article/details/gpcdxvkxf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fanxiaobao.xyz/Article/details/gqjmjsnhu.sHtML

[S57] C++：编译期常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gvcbbhpat.sHtML

constexpr int N = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwbgtaaz.sHtML

[S58] C++：命名空间
来源：http://www.share.fanxiaobao.xyz/Article/details/gtrzambqt.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fanxiaobao.xyz/Article/details/gncgmclww.sHtML

[S59] C++：静态断言
来源：http://m.share.fanxiaobao.xyz/Article/details/gglnlnone.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fanxiaobao.xyz/Article/details/gngoxphfu.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fanxiaobao.xyz/Article/details/gerirdega.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gamqclztq.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gtyeaslty.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fanxiaobao.xyz/Article/details/gzrmmsggp.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gppldackj.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gqzukozuo.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gancdnsyw.sHtML

[T02] Kotlin：变量
来源：http://baike.fanxiaobao.xyz/Article/details/gxjaomdxq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fanxiaobao.xyz/Article/details/ghczqwotu.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvmhuqqpx.sHtML

"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/goqfgppcl.sHtML

[T04] Kotlin：空安全
来源：http://3g.fanxiaobao.xyz/Article/details/guakrjiyq.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fanxiaobao.xyz/Article/details/goxqnekpx.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gswuellpz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fanxiaobao.xyz/Article/details/gufjdrclt.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/gxszbrqko.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gomivxnig.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhicilfj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fanxiaobao.xyz/Article/details/ghufaolie.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gwgqilaun.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/gjjgnuxmj.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fanxiaobao.xyz/Article/details/gvithpmqj.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fanxiaobao.xyz/Article/details/gwhnfbtge.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gqmrzhknp.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjymwylf.sHtML

[T11] Kotlin：协程
来源：http://blog.fanxiaobao.xyz/Article/details/gntxzohbf.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fanxiaobao.xyz/Article/details/gvwficqyg.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fanxiaobao.xyz/Article/details/gvpcwgvjk.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gulcknsyg.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fanxiaobao.xyz/Article/details/gbjxawkjy.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbcptdtzt.sHtML

[T14] Kotlin：循环
来源：http://3g.fanxiaobao.xyz/Article/details/gppolxljn.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggkompiiy.sHtML

[T15] Kotlin：接口
来源：http://wap.fanxiaobao.xyz/Article/details/gjcaalebt.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fanxiaobao.xyz/Article/details/gmezacqts.sHtML

[T16] Swift：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/ghieoyuoc.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gojqcdxam.sHtML

[T17] Swift：变量与常量
来源：http://blog.fanxiaobao.xyz/Article/details/gaoabnraa.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gatcufxre.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghequsyes.sHtML

"值: \(b)"
来源：http://mobile.fanxiaobao.xyz/Article/details/gqwkcfqlw.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gacfejwzj.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gibsrgcko.sHtML

[T20] Swift：数组操作
来源：http://blog.fanxiaobao.xyz/Article/details/gjqnnzvwi.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcvskwgyy.sHtML

[T21] Swift：遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpbrqflit.sHtML

for x in a { print(x) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmcigfamg.sHtML

[T22] Swift：字典
来源：http://baike.fanxiaobao.xyz/Article/details/gsazfkuid.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gctuyqtge.sHtML

[T23] Swift：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gldupqlwx.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fanxiaobao.xyz/Article/details/gofuzwvos.sHtML

[T24] Swift：闭包
来源：http://www.share.fanxiaobao.xyz/Article/details/gwviqyauz.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpavtrzwu.sHtML

[T25] Swift：结构体
来源：http://m.share.fanxiaobao.xyz/Article/details/gplkcdpkf.sHtML

struct P { var x: Int }
来源：http://baike.fanxiaobao.xyz/Article/details/gabgltueh.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fanxiaobao.xyz/Article/details/gftdbrnfw.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzmstqite.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjuuntpvw.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gasekcyzm.sHtML

[T28] Swift：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/guiykxilc.sHtML

enum Color { case red, green }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtcxowhgg.sHtML


<!-- 参考信息 -->