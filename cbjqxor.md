代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.hesvh.cn/Article/details/gyywstoii.sHtML

[R26] 命令替换
来源：http://baike.hesvh.cn/Article/details/gechshfnr.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.hesvh.cn/Article/details/gtqpuzpnp.sHtML

[R27] 算术展开
来源：http://3g.zdbjq.cn/Article/details/grhukrjbq.sHtML

echo $((1 + 2 * 3))
来源：http://wap.hesvh.cn/Article/details/givhlskpt.sHtML

[R28] 浮点运算
来源：http://3g.fehbvm.com/Article/details/gmxyosdtz.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.hesvh.cn/Article/details/gnanqvapi.sHtML

[R29] 定义函数
来源：http://www.m.share.hesvh.cn/Article/details/gfbnrqopt.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fehbvm.com/Article/details/gyuxarraq.sHtML

[R30] 函数返回状态码
来源：http://read.share.fehbvm.com/Article/details/gwgkjzvxh.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fehbvm.com/Article/details/gqgtidvtt.sHtML

[R31] 局部变量
来源：http://www.share.zdbjq.cn/Article/details/grgzlbsor.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.hesvh.cn/Article/details/gdexfkoqh.sHtML

[R32] 参数个数校验
来源：http://www.blog.hesvh.cn/Article/details/gzfvjegyo.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/geukjzbtv.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.hesvh.cn/Article/details/gcygzfqol.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fehbvm.com/Article/details/gplckaert.sHtML

[R34] 退出时清理
来源：http://blog.hesvh.cn/Article/details/grjqbkwjn.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/gzhwghdco.sHtML

[R35] 后台执行并等待
来源：http://3g.fehbvm.com/Article/details/gchgfagms.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.hesvh.cn/Article/details/gxlwawkxw.sHtML

[R36] 并发执行多个任务
来源：http://read.share.zdbjq.cn/Article/details/gjiszomfd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fehbvm.com/Article/details/gkwdcwowf.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.zdbjq.cn/Article/details/gqyokqbic.sHtML

files=$(ls -1)
来源：http://mobile.zdbjq.cn/Article/details/gdkbotuvv.sHtML

[R38] 管道串联
来源：http://baike.fehbvm.com/Article/details/gcorzkcrp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.zdbjq.cn/Article/details/glkmplgjw.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fehbvm.com/Article/details/gapurfjza.sHtML

cmd > out.log 2>&1
来源：http://3g.hesvh.cn/Article/details/gfglmfwzg.sHtML

[R40] 追加写日志
来源：http://www.m.share.hesvh.cn/Article/details/gsfjjlzeo.sHtML

echo "log" >> out.log
来源：http://baike.hesvh.cn/Article/details/gyacxnrew.sHtML

[R41] 丢弃输出
来源：http://wap.fehbvm.com/Article/details/gukpejena.sHtML

cmd >/dev/null 2>&1
来源：http://blog.zdbjq.cn/Article/details/gtkvodcqm.sHtML

[R42] 输入重定向
来源：http://www.m.share.hesvh.cn/Article/details/ghlyffleb.sHtML

wc -l < a.txt
来源：http://blog.hesvh.cn/Article/details/gooorwsee.sHtML

[R43] 按名字查找文件
来源：http://3g.fehbvm.com/Article/details/gqxmduosd.sHtML

find . -name "*.log" -type f
来源：http://baike.hesvh.cn/Article/details/gfdonaacw.sHtML

[R44] 按修改时间查找
来源：http://baike.zdbjq.cn/Article/details/grochswmy.sHtML

find . -mtime -7 -type f
来源：http://baike.zdbjq.cn/Article/details/gktizhbwi.sHtML

[R45] 批量删除
来源：http://mobile.zdbjq.cn/Article/details/gxxkastbm.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.zdbjq.cn/Article/details/gluibiefc.sHtML

[R46] 递归替换文件内容
来源：http://baike.fehbvm.com/Article/details/gdsdcrmbi.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fehbvm.com/Article/details/gyuklmpcv.sHtML

[R47] sed 单行替换
来源：http://read.share.hesvh.cn/Article/details/gxuhjhncm.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.hesvh.cn/Article/details/gwgmahixv.sHtML

[R48] awk 取指定列
来源：http://www.m.share.zdbjq.cn/Article/details/gedijonvp.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gtdunrvkp.sHtML

[R49] awk 带条件
来源：http://www.blog.fehbvm.com/Article/details/gimpggcpi.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fehbvm.com/Article/details/gqaqyjmse.sHtML

[R50] awk 求和
来源：http://www.blog.fehbvm.com/Article/details/gsdestnls.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.hesvh.cn/Article/details/gsupvsudc.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.zdbjq.cn/Article/details/gsigrssjv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.zdbjq.cn/Article/details/gyxewnluh.sHtML

[R52] 统计行数
来源：http://www.m.share.fehbvm.com/Article/details/gdkjayvlx.sHtML

wc -l a.txt
来源：http://www.share.hesvh.cn/Article/details/grnqgvzqe.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fehbvm.com/Article/details/gruvixavj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.hesvh.cn/Article/details/gxdamtgnz.sHtML

[R54] 比较两个文件
来源：http://www.share.zdbjq.cn/Article/details/gbfeitfos.sHtML

diff a.txt b.txt
来源：http://m.share.fehbvm.com/Article/details/gmefiszxs.sHtML

[R55] 压缩与解压
来源：http://baike.fehbvm.com/Article/details/glqlaesao.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.zdbjq.cn/Article/details/gahytactp.sHtML

[R56] 远程拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gacvlupmb.sHtML

scp file user@host:/path/
来源：http://baike.fehbvm.com/Article/details/glysdyrlq.sHtML

[R57] 远程执行命令
来源：http://m.share.fehbvm.com/Article/details/guyrtxxjd.sHtML

ssh user@host 'uptime'
来源：http://3g.hesvh.cn/Article/details/gvqcebdbh.sHtML

[R58] 下载文件
来源：http://read.share.fehbvm.com/Article/details/gafgvincu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.hesvh.cn/Article/details/gcibqlcse.sHtML

[R59] 发 POST JSON
来源：http://read.share.hesvh.cn/Article/details/gbetrtaxf.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.hesvh.cn/Article/details/gnpmaarlw.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/gzykkgked.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.hesvh.cn/Article/details/grcztgzwr.sHtML

[R61] 磁盘占用
来源：http://mobile.hesvh.cn/Article/details/grctowlca.sHtML

df -h;  du -sh *
来源：http://blog.fehbvm.com/Article/details/gkvgcpyry.sHtML

[R62] 找最占空间的文件
来源：http://blog.fehbvm.com/Article/details/gwgranmpo.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.hesvh.cn/Article/details/gdmqfufws.sHtML

[R63] 内存与进程
来源：http://www.m.share.zdbjq.cn/Article/details/gjujmioeg.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.hesvh.cn/Article/details/gwxvnvirz.sHtML

[R64] 结束进程
来源：http://www.blog.fehbvm.com/Article/details/ggimarjiz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fehbvm.com/Article/details/gsocejbwx.sHtML

[R65] 查看端口占用
来源：http://blog.fehbvm.com/Article/details/gexegvyud.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.hesvh.cn/Article/details/ghozphwsb.sHtML

[R66] 定时任务
来源：http://www.blog.hesvh.cn/Article/details/gdvliotfe.sHtML

crontab -e;  crontab -l
来源：http://read.share.zdbjq.cn/Article/details/gkgdynifk.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.hesvh.cn/Article/details/gwpvdtiiz.sHtML

openssl rand -hex 16
来源：http://3g.hesvh.cn/Article/details/goyqzzazn.sHtML

[R68] 计算文件校验值
来源：http://www.share.fehbvm.com/Article/details/gepaikawr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fehbvm.com/Article/details/gwkvfjmwj.sHtML

[R69] 生成随机密码
来源：http://baike.fehbvm.com/Article/details/gysiluwok.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fehbvm.com/Article/details/gxnkiofex.sHtML

[R70] 时间戳与互转
来源：http://www.share.fehbvm.com/Article/details/gecautiww.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.zdbjq.cn/Article/details/gthirzxoj.sHtML

[R71] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/geoumkluh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.zdbjq.cn/Article/details/gvcqpblir.sHtML

[R72] 等待端口就绪
来源：http://wap.hesvh.cn/Article/details/ggooulvey.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/gmvicgfxs.sHtML

[R73] 分割大日志
来源：http://3g.hesvh.cn/Article/details/gpzpugbgb.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.zdbjq.cn/Article/details/gznbsnfiz.sHtML

[R74] 批量重命名
来源：http://www.blog.hesvh.cn/Article/details/gtdizpjho.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.hesvh.cn/Article/details/gfspmuzcl.sHtML

[R75] 导出环境变量
来源：http://blog.zdbjq.cn/Article/details/gbsoxhruo.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fehbvm.com/Article/details/gomotlwnn.sHtML

[R76] 使用临时文件
来源：http://blog.fehbvm.com/Article/details/gepzdofzg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/gkfleygww.sHtML

[R77] 读取用户输入
来源：http://mobile.zdbjq.cn/Article/details/gkiuwttyn.sHtML

read -rp "请输入: " ans
来源：http://www.blog.hesvh.cn/Article/details/gumpfpzgk.sHtML

[R78] 交互式菜单
来源：http://wap.hesvh.cn/Article/details/gnqtazzzu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.zdbjq.cn/Article/details/gzopdedth.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fehbvm.com/Article/details/ggftwatdt.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fehbvm.com/Article/details/gaubcrunj.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fehbvm.com/Article/details/gipmncdcl.sHtML

time ./run.sh
来源：http://m.share.hesvh.cn/Article/details/gmstlurjc.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ghnmrticx.sHtML

S. C / C++ 专题
来源：http://www.share.hesvh.cn/Article/details/gsqdgwpnl.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gccctxfac.sHtML

[S01] C：Hello World
来源：http://read.share.fehbvm.com/Article/details/gekbuwnuu.sHtML

#include <stdio.h>
来源：http://www.blog.zdbjq.cn/Article/details/gneqfrbne.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.hesvh.cn/Article/details/gzlseynih.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.zdbjq.cn/Article/details/gtbkklscn.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.hesvh.cn/Article/details/guzerkzig.sHtML

[S03] C：读入整数
来源：http://www.share.hesvh.cn/Article/details/gjktjsdrs.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fehbvm.com/Article/details/gebbizvge.sHtML

[S04] C：字符串复制
来源：http://www.blog.hesvh.cn/Article/details/ggwbnwzzj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.zdbjq.cn/Article/details/gztvmwufn.sHtML

[S05] C：字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/gcmuuzvga.sHtML

strlen(s)
来源：http://mobile.fehbvm.com/Article/details/gnliavftm.sHtML

[S06] C：字符串比较
来源：http://wap.hesvh.cn/Article/details/gtvrkiahz.sHtML

strcmp(a, b) == 0
来源：http://wap.hesvh.cn/Article/details/gvsiieapg.sHtML

[S07] C：数组遍历求和
来源：http://mobile.zdbjq.cn/Article/details/gsycxcobd.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.zdbjq.cn/Article/details/gmkcywsnf.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.zdbjq.cn/Article/details/gjqokblwg.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.zdbjq.cn/Article/details/goqlvsqns.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.hesvh.cn/Article/details/gvxiyiatw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.zdbjq.cn/Article/details/gznujojnm.sHtML

[S10] C：指针与解引用
来源：http://baike.fehbvm.com/Article/details/gjjldgiba.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.zdbjq.cn/Article/details/gcyspzzpa.sHtML

[S11] C：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gchdqbeuj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.hesvh.cn/Article/details/gmgipmswp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fehbvm.com/Article/details/gmitnzraq.sHtML

fclose(f);
来源：http://blog.fehbvm.com/Article/details/gyezlroox.sHtML

[S12] C：写文件
来源：http://www.blog.zdbjq.cn/Article/details/gjcsswrsq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/gpzzvwoik.sHtML

[S13] C：宏定义
来源：http://mobile.hesvh.cn/Article/details/gmykvoosf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fehbvm.com/Article/details/gtzqfjhtu.sHtML

[S14] C：枚举
来源：http://blog.zdbjq.cn/Article/details/giajcadeb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.zdbjq.cn/Article/details/gxkyldzwd.sHtML

[S15] C：类型转换
来源：http://mobile.hesvh.cn/Article/details/gxnocaecl.sHtML

(double) a / b
来源：http://wap.fehbvm.com/Article/details/gqelmpoxh.sHtML

[S16] C：位操作置位
来源：http://mobile.fehbvm.com/Article/details/gvldwrzou.sHtML

x |= (1 << 3);
来源：http://baike.hesvh.cn/Article/details/gpwnkoafn.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gttlukymd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.zdbjq.cn/Article/details/glhscxkpz.sHtML

[S18] C：命令行参数
来源：http://baike.zdbjq.cn/Article/details/gqudjmtrw.sHtML

int main(int argc, char **argv)
来源：http://wap.hesvh.cn/Article/details/glmbsfyka.sHtML

[S19] C：快速排序
来源：http://baike.fehbvm.com/Article/details/gthuuhico.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/glfgjdmqm.sHtML

[S20] C：二分查找
来源：http://www.m.share.fehbvm.com/Article/details/gdkuvcqbu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gqwislnzt.sHtML

[S21] C：字符类别判断
来源：http://m.share.hesvh.cn/Article/details/grnxkfoqa.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.zdbjq.cn/Article/details/guntnqaof.sHtML

[S22] C：字符串转数字
来源：http://3g.zdbjq.cn/Article/details/gyctntvpm.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.hesvh.cn/Article/details/gvcwfbnmy.sHtML

[S23] C：随机数
来源：http://read.share.fehbvm.com/Article/details/gxgavovmb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.zdbjq.cn/Article/details/gopsujwoc.sHtML

[S24] C：获取本地时间
来源：http://wap.zdbjq.cn/Article/details/gywhnxskp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.hesvh.cn/Article/details/gnjokleoo.sHtML

[S25] C：内存拷贝
来源：http://www.share.zdbjq.cn/Article/details/gnbirlsvd.sHtML

memcpy(dst, src, n);
来源：http://baike.zdbjq.cn/Article/details/gqezttbnj.sHtML

[S26] C：内存清零
来源：http://baike.hesvh.cn/Article/details/grmvnbppr.sHtML

memset(a, 0, sizeof a);
来源：http://blog.zdbjq.cn/Article/details/gewmtqvvj.sHtML

[S27] C：定义常量
来源：http://m.share.hesvh.cn/Article/details/ggxdajdbi.sHtML

const double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gnwfgrjoc.sHtML

[S28] C：静态变量
来源：http://baike.fehbvm.com/Article/details/grsyeacax.sHtML

static int counter = 0;
来源：http://3g.hesvh.cn/Article/details/goiebcfnz.sHtML

[S29] C：变参函数
来源：http://www.m.share.fehbvm.com/Article/details/gkgrgegeb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.hesvh.cn/Article/details/gfnbptvzh.sHtML

[S30] C：头文件保护
来源：http://mobile.hesvh.cn/Article/details/gtzazxltd.sHtML

#ifndef X_H
来源：http://www.share.hesvh.cn/Article/details/gsnialbur.sHtML

#define X_H
来源：http://www.blog.zdbjq.cn/Article/details/gykyhruzl.sHtML

#endif
来源：http://www.share.zdbjq.cn/Article/details/gkixvflfm.sHtML

[S31] C++：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gxfioruha.sHtML

#include <iostream>
来源：http://blog.zdbjq.cn/Article/details/gkeculsuc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.zdbjq.cn/Article/details/gyhmhtmxu.sHtML

[S32] C++：字符串
来源：http://read.share.fehbvm.com/Article/details/gmdbvdugx.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fehbvm.com/Article/details/ggdrdgdit.sHtML

[S33] C++：vector 增删
来源：http://3g.fehbvm.com/Article/details/gvkdtxzdv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fehbvm.com/Article/details/gtsenyamj.sHtML

[S34] C++：遍历 vector
来源：http://wap.fehbvm.com/Article/details/gnzxxjnbn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fehbvm.com/Article/details/gygqyomae.sHtML

[S35] C++：map
来源：http://mobile.zdbjq.cn/Article/details/gmutjegpg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/guxyatdrc.sHtML

[S36] C++：unordered_map
来源：http://www.blog.zdbjq.cn/Article/details/ghuyljtxd.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/govjdhhba.sHtML

[S37] C++：set
来源：http://3g.hesvh.cn/Article/details/ggabunzyi.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fehbvm.com/Article/details/gosqjcimz.sHtML

[S38] C++：排序
来源：http://wap.hesvh.cn/Article/details/grayftmmy.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.hesvh.cn/Article/details/gnhqzxlaj.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.zdbjq.cn/Article/details/gpunyqsph.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.hesvh.cn/Article/details/gsfzswbgk.sHtML

[S40] C++：查找元素
来源：http://baike.zdbjq.cn/Article/details/gwsiwtsya.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.zdbjq.cn/Article/details/gdigrwedc.sHtML

[S41] C++：类与构造函数
来源：http://wap.zdbjq.cn/Article/details/ghhbobdzb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fehbvm.com/Article/details/gyjdhgani.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.zdbjq.cn/Article/details/gsqnjawhf.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fehbvm.com/Article/details/gtwhauwle.sHtML

[S43] C++：智能指针
来源：http://baike.fehbvm.com/Article/details/gmqesxvnf.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.zdbjq.cn/Article/details/gnknccdbf.sHtML

[S44] C++：引用传参
来源：http://read.share.zdbjq.cn/Article/details/gjzzzypsq.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fehbvm.com/Article/details/gkjkklopm.sHtML

[S45] C++：lambda
来源：http://baike.hesvh.cn/Article/details/ggyefvlop.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.hesvh.cn/Article/details/gtrlsstrx.sHtML

[S46] C++：函数模板
来源：http://read.share.zdbjq.cn/Article/details/gawqkmqof.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fehbvm.com/Article/details/gqctvbakh.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fehbvm.com/Article/details/gxgahytyq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.hesvh.cn/Article/details/gagslcdli.sHtML

[S48] C++：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gxfgjlfli.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fehbvm.com/Article/details/gcfpttzox.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fehbvm.com/Article/details/gwjaoupsm.sHtML

[S49] C++：写文件
来源：http://wap.hesvh.cn/Article/details/gzuzdoxic.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fehbvm.com/Article/details/glyckpgob.sHtML

[S50] C++：格式化数字
来源：http://mobile.fehbvm.com/Article/details/glxdpebzg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fehbvm.com/Article/details/gixlagrko.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fehbvm.com/Article/details/gpmxglwro.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.hesvh.cn/Article/details/gvznykrst.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.zdbjq.cn/Article/details/gynxgdnot.sHtML

int size() const noexcept { return n_; }
来源：http://baike.hesvh.cn/Article/details/gedxagcrp.sHtML

[S53] C++：移动语义
来源：http://3g.fehbvm.com/Article/details/gwpimqagq.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fehbvm.com/Article/details/gqmguhcej.sHtML

[S54] C++：异常处理
来源：http://m.share.hesvh.cn/Article/details/ghcaipzwu.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.hesvh.cn/Article/details/ganpnrune.sHtML

[S55] C++：结构化绑定
来源：http://read.share.hesvh.cn/Article/details/guisgcgcs.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fehbvm.com/Article/details/gjhglfgnm.sHtML

[S56] C++：optional
来源：http://blog.zdbjq.cn/Article/details/gidradvwc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.hesvh.cn/Article/details/gqxbklmix.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.hesvh.cn/Article/details/gwzrdesqx.sHtML

constexpr int N = 10;
来源：http://m.share.hesvh.cn/Article/details/gdsnwxyep.sHtML

[S58] C++：命名空间
来源：http://mobile.hesvh.cn/Article/details/gurhdboeu.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fehbvm.com/Article/details/gkmwlrogh.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fehbvm.com/Article/details/gtxnsoqme.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.zdbjq.cn/Article/details/gemmjmrco.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/glqjhqwgj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fehbvm.com/Article/details/gwuzleqez.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gghniijyp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fehbvm.com/Article/details/ggjgitxbk.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gcstzfsms.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.hesvh.cn/Article/details/gkfneofal.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/grbwfgbgz.sHtML

[T02] Kotlin：变量
来源：http://baike.zdbjq.cn/Article/details/gqfaicxkn.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.hesvh.cn/Article/details/gvmouwfkj.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.hesvh.cn/Article/details/gvhyqurzg.sHtML

"值: $b"
来源：http://mobile.hesvh.cn/Article/details/giizzkuoh.sHtML

[T04] Kotlin：空安全
来源：http://blog.zdbjq.cn/Article/details/gedwgeivi.sHtML

val n: String? = null;  n?.length
来源：http://mobile.hesvh.cn/Article/details/gnmqnmnng.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.hesvh.cn/Article/details/gbhkkxoiq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.zdbjq.cn/Article/details/gipxdgcpt.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/gctqzknpk.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gwxsbotsz.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.zdbjq.cn/Article/details/ghxffzuxa.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.hesvh.cn/Article/details/glwdkvkgm.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fehbvm.com/Article/details/gyryoteab.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fehbvm.com/Article/details/gapaakjss.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.hesvh.cn/Article/details/ghwuxzsgw.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.hesvh.cn/Article/details/gnspcmhvu.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fehbvm.com/Article/details/gmvwebmjt.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.hesvh.cn/Article/details/guxzkgnqp.sHtML

[T11] Kotlin：协程
来源：http://read.share.fehbvm.com/Article/details/gwmkwtynk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.hesvh.cn/Article/details/gkfieukbf.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fehbvm.com/Article/details/ggrcompxj.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gtgwldydq.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.zdbjq.cn/Article/details/gwtxfjibi.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.hesvh.cn/Article/details/gtwtxaeyb.sHtML

[T14] Kotlin：循环
来源：http://www.blog.zdbjq.cn/Article/details/gkzixubpr.sHtML

for (i in 1..10) println(i)
来源：http://baike.zdbjq.cn/Article/details/gfbmvxdrf.sHtML

[T15] Kotlin：接口
来源：http://blog.zdbjq.cn/Article/details/ghxdluopt.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fehbvm.com/Article/details/grouilgap.sHtML

[T16] Swift：Hello World
来源：http://baike.zdbjq.cn/Article/details/gwjalzskf.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gojonsmmj.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.zdbjq.cn/Article/details/gukgzoghe.sHtML

var a = 1;  let b = 2
来源：http://baike.fehbvm.com/Article/details/gijrrqxjb.sHtML

[T18] Swift：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/ggchdnwif.sHtML

"值: \(b)"
来源：http://3g.fehbvm.com/Article/details/gkxpwayjx.sHtML

[T19] Swift：可选绑定
来源：http://www.share.hesvh.cn/Article/details/grbresszq.sHtML

if let n = opt { print(n) }
来源：http://baike.fehbvm.com/Article/details/geodmaqnj.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.hesvh.cn/Article/details/gaegrghgs.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.hesvh.cn/Article/details/gnxvfvwbp.sHtML

[T21] Swift：遍历
来源：http://read.share.zdbjq.cn/Article/details/gdfixrwuz.sHtML

for x in a { print(x) }
来源：http://3g.hesvh.cn/Article/details/gylafulqx.sHtML

[T22] Swift：字典
来源：http://3g.fehbvm.com/Article/details/gimpxohqy.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gtluwktrh.sHtML

[T23] Swift：函数
来源：http://wap.zdbjq.cn/Article/details/giyqaotvt.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.hesvh.cn/Article/details/gtjaergwy.sHtML

[T24] Swift：闭包
来源：http://www.share.hesvh.cn/Article/details/gppwbjgec.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.hesvh.cn/Article/details/gspdhhqiq.sHtML

[T25] Swift：结构体
来源：http://3g.hesvh.cn/Article/details/gamsixadd.sHtML

struct P { var x: Int }
来源：http://mobile.fehbvm.com/Article/details/gakhuuwru.sHtML

[T26] Swift：类与重写
来源：http://m.share.fehbvm.com/Article/details/gllktntri.sHtML

class A: Base { override func f() {} }
来源：http://mobile.hesvh.cn/Article/details/gmchiwalz.sHtML

[T27] Swift：错误处理
来源：http://m.share.zdbjq.cn/Article/details/gbketmiuo.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fehbvm.com/Article/details/gkjlqngcy.sHtML

[T28] Swift：枚举
来源：http://baike.hesvh.cn/Article/details/gzmdsawal.sHtML

enum Color { case red, green }
来源：http://3g.zdbjq.cn/Article/details/gsssyhsse.sHtML


<!-- 参考信息 -->