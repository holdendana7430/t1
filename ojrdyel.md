代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://blog.zdbjq.cn/Article/details/gesanoyxw.sHtML

[R32] 参数个数校验
来源：http://www.share.hesvh.cn/Article/details/govjvtdxy.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gdobmpzke.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fehbvm.com/Article/details/gicwbeiqc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.hesvh.cn/Article/details/gurffbilo.sHtML

[R34] 退出时清理
来源：http://read.share.fehbvm.com/Article/details/gdpgjjvqh.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/gaxjocane.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fehbvm.com/Article/details/gikokkmpt.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.hesvh.cn/Article/details/gdrugjjzw.sHtML

[R36] 并发执行多个任务
来源：http://read.share.hesvh.cn/Article/details/gbekkrknd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.zdbjq.cn/Article/details/gifpfsfyb.sHtML

[R37] 把输出赋给变量
来源：http://www.share.hesvh.cn/Article/details/ggexmeuwb.sHtML

files=$(ls -1)
来源：http://mobile.zdbjq.cn/Article/details/gonsfasrt.sHtML

[R38] 管道串联
来源：http://www.share.hesvh.cn/Article/details/gqwjpwepv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fehbvm.com/Article/details/gjnevfgpa.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.hesvh.cn/Article/details/gbchihbua.sHtML

cmd > out.log 2>&1
来源：http://blog.fehbvm.com/Article/details/goewkuzau.sHtML

[R40] 追加写日志
来源：http://m.share.zdbjq.cn/Article/details/gtbnxgsvc.sHtML

echo "log" >> out.log
来源：http://www.blog.hesvh.cn/Article/details/gsrikggpi.sHtML

[R41] 丢弃输出
来源：http://www.share.zdbjq.cn/Article/details/galcuslth.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fehbvm.com/Article/details/gdloolxrb.sHtML

[R42] 输入重定向
来源：http://mobile.fehbvm.com/Article/details/gvvmaygzh.sHtML

wc -l < a.txt
来源：http://www.share.zdbjq.cn/Article/details/gkpvgjojh.sHtML

[R43] 按名字查找文件
来源：http://read.share.hesvh.cn/Article/details/gdpvwxjqx.sHtML

find . -name "*.log" -type f
来源：http://baike.zdbjq.cn/Article/details/gwegovkkj.sHtML

[R44] 按修改时间查找
来源：http://read.share.hesvh.cn/Article/details/gzogjsssl.sHtML

find . -mtime -7 -type f
来源：http://3g.zdbjq.cn/Article/details/gucnizkux.sHtML

[R45] 批量删除
来源：http://baike.fehbvm.com/Article/details/gzevuvitg.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.zdbjq.cn/Article/details/glpgdtbid.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.zdbjq.cn/Article/details/gmtscxcij.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fehbvm.com/Article/details/gmtthjvmn.sHtML

[R47] sed 单行替换
来源：http://mobile.hesvh.cn/Article/details/gizkhiwfs.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.hesvh.cn/Article/details/gljuggjhj.sHtML

[R48] awk 取指定列
来源：http://mobile.zdbjq.cn/Article/details/gxwfmzwxf.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fehbvm.com/Article/details/gwnkjzicb.sHtML

[R49] awk 带条件
来源：http://www.m.share.fehbvm.com/Article/details/gcbilzbap.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.hesvh.cn/Article/details/gggbwowop.sHtML

[R50] awk 求和
来源：http://read.share.hesvh.cn/Article/details/ggjwkvlrk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.zdbjq.cn/Article/details/gmrycjilr.sHtML

[R51] 排序去重取前几
来源：http://m.share.fehbvm.com/Article/details/gcsertsmr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.hesvh.cn/Article/details/ghfagwmhs.sHtML

[R52] 统计行数
来源：http://www.m.share.hesvh.cn/Article/details/gqlpoxvdh.sHtML

wc -l a.txt
来源：http://wap.hesvh.cn/Article/details/gxwvpmjop.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.zdbjq.cn/Article/details/gnismfcwl.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.zdbjq.cn/Article/details/gzdthrnlv.sHtML

[R54] 比较两个文件
来源：http://read.share.zdbjq.cn/Article/details/gwujylfmj.sHtML

diff a.txt b.txt
来源：http://read.share.zdbjq.cn/Article/details/ghbahrnoc.sHtML

[R55] 压缩与解压
来源：http://3g.zdbjq.cn/Article/details/gqxliodwd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.hesvh.cn/Article/details/gveujghhy.sHtML

[R56] 远程拷贝
来源：http://www.m.share.hesvh.cn/Article/details/getmhqxzn.sHtML

scp file user@host:/path/
来源：http://wap.fehbvm.com/Article/details/glixlyoan.sHtML

[R57] 远程执行命令
来源：http://www.blog.hesvh.cn/Article/details/grjxbxylo.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fehbvm.com/Article/details/gmrohthro.sHtML

[R58] 下载文件
来源：http://baike.hesvh.cn/Article/details/gwlxeyzyi.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.hesvh.cn/Article/details/gzzitijpz.sHtML

[R59] 发 POST JSON
来源：http://www.blog.hesvh.cn/Article/details/gimxmpwlu.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.hesvh.cn/Article/details/gvtkndnoq.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/gbinszeis.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.zdbjq.cn/Article/details/grzffuzhu.sHtML

[R61] 磁盘占用
来源：http://read.share.hesvh.cn/Article/details/gudjvgytw.sHtML

df -h;  du -sh *
来源：http://read.share.hesvh.cn/Article/details/geawmvhzd.sHtML

[R62] 找最占空间的文件
来源：http://www.share.hesvh.cn/Article/details/ghziaahkx.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fehbvm.com/Article/details/gmojzjcri.sHtML

[R63] 内存与进程
来源：http://www.share.hesvh.cn/Article/details/gvgrxntme.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.zdbjq.cn/Article/details/gkuityomh.sHtML

[R64] 结束进程
来源：http://mobile.zdbjq.cn/Article/details/guoupaodv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.hesvh.cn/Article/details/gdhnmdchm.sHtML

[R65] 查看端口占用
来源：http://m.share.hesvh.cn/Article/details/gvrifvioe.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.hesvh.cn/Article/details/gsiakmhhb.sHtML

[R66] 定时任务
来源：http://www.share.fehbvm.com/Article/details/gxggnwehz.sHtML

crontab -e;  crontab -l
来源：http://m.share.zdbjq.cn/Article/details/glottrlpp.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fehbvm.com/Article/details/gntmkhywq.sHtML

openssl rand -hex 16
来源：http://www.share.zdbjq.cn/Article/details/gyebebnct.sHtML

[R68] 计算文件校验值
来源：http://www.share.hesvh.cn/Article/details/gxghocbyx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fehbvm.com/Article/details/gqizjjiyb.sHtML

[R69] 生成随机密码
来源：http://3g.fehbvm.com/Article/details/gplavzhld.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.hesvh.cn/Article/details/geessesir.sHtML

[R70] 时间戳与互转
来源：http://blog.zdbjq.cn/Article/details/gdxsagieq.sHtML

date +%s;  date -d @1700000000
来源：http://blog.zdbjq.cn/Article/details/gaqswzvyu.sHtML

[R71] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gtonghgbo.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.zdbjq.cn/Article/details/gmlhyqrji.sHtML

[R72] 等待端口就绪
来源：http://read.share.fehbvm.com/Article/details/gtjhojqeu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/gnytqnjji.sHtML

[R73] 分割大日志
来源：http://www.m.share.zdbjq.cn/Article/details/gtglqzpmt.sHtML

split -l 1000 big.log part_
来源：http://mobile.fehbvm.com/Article/details/gzzvqqjah.sHtML

[R74] 批量重命名
来源：http://www.share.zdbjq.cn/Article/details/gqskblaix.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fehbvm.com/Article/details/gyalulsje.sHtML

[R75] 导出环境变量
来源：http://3g.hesvh.cn/Article/details/glbttsyaj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.hesvh.cn/Article/details/gxydudxbi.sHtML

[R76] 使用临时文件
来源：http://m.share.fehbvm.com/Article/details/guttmkdgd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/gmdwvgoje.sHtML

[R77] 读取用户输入
来源：http://wap.hesvh.cn/Article/details/gexnakwpe.sHtML

read -rp "请输入: " ans
来源：http://3g.hesvh.cn/Article/details/gvxjzomjm.sHtML

[R78] 交互式菜单
来源：http://3g.fehbvm.com/Article/details/geopekzmg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.hesvh.cn/Article/details/gyqmqtqup.sHtML

[R79] 解析命令行选项
来源：http://www.share.hesvh.cn/Article/details/gakjgsmax.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.zdbjq.cn/Article/details/gmzojdyhv.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fehbvm.com/Article/details/gcfxjifcn.sHtML

time ./run.sh
来源：http://www.blog.zdbjq.cn/Article/details/gyxgxzpyy.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gynysxffz.sHtML

S. C / C++ 专题
来源：http://wap.fehbvm.com/Article/details/gykjhetlq.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/guxndmaag.sHtML

[S01] C：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gkmwmbhri.sHtML

#include <stdio.h>
来源：http://www.share.zdbjq.cn/Article/details/gaginfvjv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.zdbjq.cn/Article/details/gawixcjdh.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.hesvh.cn/Article/details/gcalnybkn.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.hesvh.cn/Article/details/gppnogbbs.sHtML

[S03] C：读入整数
来源：http://3g.fehbvm.com/Article/details/gxnuxlroe.sHtML

int x; scanf("%d", &x);
来源：http://read.share.zdbjq.cn/Article/details/gdnnzbvts.sHtML

[S04] C：字符串复制
来源：http://m.share.zdbjq.cn/Article/details/gexfjrqwo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fehbvm.com/Article/details/gilwypnso.sHtML

[S05] C：字符串长度
来源：http://www.share.fehbvm.com/Article/details/gyldlpaem.sHtML

strlen(s)
来源：http://m.share.zdbjq.cn/Article/details/geqcsqkmp.sHtML

[S06] C：字符串比较
来源：http://baike.hesvh.cn/Article/details/gviiulcwu.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.zdbjq.cn/Article/details/ggbvfrlxk.sHtML

[S07] C：数组遍历求和
来源：http://mobile.zdbjq.cn/Article/details/gdqkcpklv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.hesvh.cn/Article/details/gijqgjhpk.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.hesvh.cn/Article/details/gyggbmkzl.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.zdbjq.cn/Article/details/geqejaieb.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fehbvm.com/Article/details/gjsfedifv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fehbvm.com/Article/details/gvysuajyk.sHtML

[S10] C：指针与解引用
来源：http://www.blog.hesvh.cn/Article/details/gnzzfsvhp.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.hesvh.cn/Article/details/grmzqbctp.sHtML

[S11] C：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gboqqibtf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.hesvh.cn/Article/details/gmojsjbqb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.hesvh.cn/Article/details/giwyohupw.sHtML

fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/gbiqnfyll.sHtML

[S12] C：写文件
来源：http://www.blog.fehbvm.com/Article/details/gflzoxqvw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fehbvm.com/Article/details/gjghlloyj.sHtML

[S13] C：宏定义
来源：http://m.share.fehbvm.com/Article/details/gvdydavsl.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fehbvm.com/Article/details/gipmpfcbi.sHtML

[S14] C：枚举
来源：http://3g.hesvh.cn/Article/details/gxxuemzpg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fehbvm.com/Article/details/gbmbypkym.sHtML

[S15] C：类型转换
来源：http://www.blog.hesvh.cn/Article/details/gncqjgtxq.sHtML

(double) a / b
来源：http://read.share.hesvh.cn/Article/details/gwoarssnh.sHtML

[S16] C：位操作置位
来源：http://m.share.zdbjq.cn/Article/details/gnqcnebcl.sHtML

x |= (1 << 3);
来源：http://m.share.hesvh.cn/Article/details/gpepiprlh.sHtML

[S17] C：安全拼接字符串
来源：http://wap.hesvh.cn/Article/details/gbtckfmys.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.hesvh.cn/Article/details/gceavjhwy.sHtML

[S18] C：命令行参数
来源：http://baike.fehbvm.com/Article/details/gmccbuhxp.sHtML

int main(int argc, char **argv)
来源：http://mobile.fehbvm.com/Article/details/ghzhibybx.sHtML

[S19] C：快速排序
来源：http://www.m.share.fehbvm.com/Article/details/gnedvjsnw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/gzwgupuqx.sHtML

[S20] C：二分查找
来源：http://www.share.hesvh.cn/Article/details/gqgllrizy.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gcooudveo.sHtML

[S21] C：字符类别判断
来源：http://m.share.hesvh.cn/Article/details/gvznycasy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.hesvh.cn/Article/details/grjydhffq.sHtML

[S22] C：字符串转数字
来源：http://www.share.fehbvm.com/Article/details/gqxxclkyq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.hesvh.cn/Article/details/ggjzlyclo.sHtML

[S23] C：随机数
来源：http://www.m.share.fehbvm.com/Article/details/gsymrulob.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.zdbjq.cn/Article/details/gagjwxhda.sHtML

[S24] C：获取本地时间
来源：http://www.share.zdbjq.cn/Article/details/gnlhvylbc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.zdbjq.cn/Article/details/grbqqdpqw.sHtML

[S25] C：内存拷贝
来源：http://m.share.hesvh.cn/Article/details/gexqqmfbu.sHtML

memcpy(dst, src, n);
来源：http://blog.hesvh.cn/Article/details/gviypmnfy.sHtML

[S26] C：内存清零
来源：http://wap.zdbjq.cn/Article/details/ggqojiydv.sHtML

memset(a, 0, sizeof a);
来源：http://blog.zdbjq.cn/Article/details/gfedtljxo.sHtML

[S27] C：定义常量
来源：http://www.m.share.zdbjq.cn/Article/details/gxunavqmy.sHtML

const double PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gkgffleiy.sHtML

[S28] C：静态变量
来源：http://read.share.fehbvm.com/Article/details/gpytmitrz.sHtML

static int counter = 0;
来源：http://3g.zdbjq.cn/Article/details/gaxztfoyr.sHtML

[S29] C：变参函数
来源：http://wap.zdbjq.cn/Article/details/gnqgavhml.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fehbvm.com/Article/details/glqeqapev.sHtML

[S30] C：头文件保护
来源：http://mobile.hesvh.cn/Article/details/ggkwprhzp.sHtML

#ifndef X_H
来源：http://www.m.share.hesvh.cn/Article/details/grggzwmnk.sHtML

#define X_H
来源：http://www.share.zdbjq.cn/Article/details/gmtmltxcf.sHtML

#endif
来源：http://www.share.zdbjq.cn/Article/details/gjhrymdrx.sHtML

[S31] C++：Hello World
来源：http://www.share.fehbvm.com/Article/details/gkwcqkkgj.sHtML

#include <iostream>
来源：http://m.share.zdbjq.cn/Article/details/gaywxglaa.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fehbvm.com/Article/details/goyvjtvqa.sHtML

[S32] C++：字符串
来源：http://read.share.fehbvm.com/Article/details/gauvdyxxc.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.zdbjq.cn/Article/details/gvsnvyvzy.sHtML

[S33] C++：vector 增删
来源：http://www.share.zdbjq.cn/Article/details/gqlnqejyx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gmavtcweq.sHtML

[S34] C++：遍历 vector
来源：http://baike.hesvh.cn/Article/details/gpaowwggr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.hesvh.cn/Article/details/gqivnbkiq.sHtML

[S35] C++：map
来源：http://mobile.fehbvm.com/Article/details/gvunmgsrp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gaiedbamw.sHtML

[S36] C++：unordered_map
来源：http://wap.fehbvm.com/Article/details/gqaqsaixm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gmeyzagbu.sHtML

[S37] C++：set
来源：http://baike.zdbjq.cn/Article/details/gkixicphy.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fehbvm.com/Article/details/gtipfejzl.sHtML

[S38] C++：排序
来源：http://read.share.zdbjq.cn/Article/details/gjuykozqb.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.zdbjq.cn/Article/details/gveftjloq.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fehbvm.com/Article/details/gnazfgawu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.zdbjq.cn/Article/details/gpixtnuaa.sHtML

[S40] C++：查找元素
来源：http://baike.hesvh.cn/Article/details/gchrapuax.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.hesvh.cn/Article/details/gggvqatzu.sHtML

[S41] C++：类与构造函数
来源：http://mobile.zdbjq.cn/Article/details/gwfkoshmy.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fehbvm.com/Article/details/gfpcwsbnk.sHtML

[S42] C++：继承与虚函数
来源：http://wap.hesvh.cn/Article/details/gwzfarlkx.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fehbvm.com/Article/details/gazumouet.sHtML

[S43] C++：智能指针
来源：http://wap.fehbvm.com/Article/details/gjnvqzqtn.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.hesvh.cn/Article/details/gvbzeewyy.sHtML

[S44] C++：引用传参
来源：http://wap.fehbvm.com/Article/details/gyqqigfke.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.zdbjq.cn/Article/details/gkimkhnzp.sHtML

[S45] C++：lambda
来源：http://m.share.fehbvm.com/Article/details/gsgqdppss.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.zdbjq.cn/Article/details/gvmkkbivv.sHtML

[S46] C++：函数模板
来源：http://m.share.fehbvm.com/Article/details/gqetkxcax.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.hesvh.cn/Article/details/gtbulapch.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fehbvm.com/Article/details/gtialifid.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.hesvh.cn/Article/details/gqjipfbvb.sHtML

[S48] C++：逐行读文件
来源：http://3g.fehbvm.com/Article/details/grypficwo.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fehbvm.com/Article/details/ghvocxeqi.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.hesvh.cn/Article/details/gececmmdw.sHtML

[S49] C++：写文件
来源：http://www.blog.hesvh.cn/Article/details/gbmvfdtbs.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.zdbjq.cn/Article/details/gtompmhfj.sHtML

[S50] C++：格式化数字
来源：http://baike.hesvh.cn/Article/details/ghklsdlsu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gckqgvhmd.sHtML

[S51] C++：显式类型转换
来源：http://blog.hesvh.cn/Article/details/gslmvqvif.sHtML

static_cast<double>(a) / b
来源：http://3g.fehbvm.com/Article/details/gugdllrdj.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.zdbjq.cn/Article/details/gdvnjhblv.sHtML

int size() const noexcept { return n_; }
来源：http://3g.zdbjq.cn/Article/details/gfmmgljkx.sHtML

[S53] C++：移动语义
来源：http://www.blog.fehbvm.com/Article/details/gvgaxmvfs.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fehbvm.com/Article/details/gapoctnpk.sHtML

[S54] C++：异常处理
来源：http://wap.fehbvm.com/Article/details/gqxjxolhy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.zdbjq.cn/Article/details/gswpiplxs.sHtML

[S55] C++：结构化绑定
来源：http://baike.zdbjq.cn/Article/details/gpterpzlk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.zdbjq.cn/Article/details/gwpwdjkph.sHtML

[S56] C++：optional
来源：http://www.m.share.zdbjq.cn/Article/details/gmznbcfch.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.zdbjq.cn/Article/details/gxcdugcyo.sHtML

[S57] C++：编译期常量
来源：http://m.share.hesvh.cn/Article/details/gkzikrdeb.sHtML

constexpr int N = 10;
来源：http://mobile.zdbjq.cn/Article/details/gxrcypcan.sHtML

[S58] C++：命名空间
来源：http://www.blog.fehbvm.com/Article/details/gasbbiaqz.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.zdbjq.cn/Article/details/gxzzjufyt.sHtML

[S59] C++：静态断言
来源：http://baike.zdbjq.cn/Article/details/gujatqvwb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fehbvm.com/Article/details/gjeiwmiou.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.hesvh.cn/Article/details/gbpmydibk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.hesvh.cn/Article/details/ggrqfbuiy.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gyyliexcj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.hesvh.cn/Article/details/gvufnxmtj.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/guyhuiuoq.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.zdbjq.cn/Article/details/godlismmu.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/gzavpbopr.sHtML

[T02] Kotlin：变量
来源：http://www.share.fehbvm.com/Article/details/gouuwnrym.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.zdbjq.cn/Article/details/gwnjqwpgq.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.zdbjq.cn/Article/details/gfyjxngtu.sHtML

"值: $b"
来源：http://blog.hesvh.cn/Article/details/giusziznu.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.hesvh.cn/Article/details/ghpwktwnf.sHtML

val n: String? = null;  n?.length
来源：http://wap.zdbjq.cn/Article/details/ghzffaauq.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fehbvm.com/Article/details/gsxldinvv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.zdbjq.cn/Article/details/gpjktbhzv.sHtML

[T06] Kotlin：集合映射
来源：http://wap.hesvh.cn/Article/details/gfunfkkqk.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gbyqflhrt.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/gfvjzoncn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fehbvm.com/Article/details/gffjdgivn.sHtML

[T08] Kotlin：数据类
来源：http://blog.fehbvm.com/Article/details/gcktymfik.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fehbvm.com/Article/details/glcdfilwf.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fehbvm.com/Article/details/gayjdzeld.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.zdbjq.cn/Article/details/gftfttquq.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.hesvh.cn/Article/details/gezpktulk.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.zdbjq.cn/Article/details/gkudyiggf.sHtML

[T11] Kotlin：协程
来源：http://wap.fehbvm.com/Article/details/grqseekca.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fehbvm.com/Article/details/guekplyvo.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.zdbjq.cn/Article/details/gcrsuaqes.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.hesvh.cn/Article/details/gdrplenqo.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fehbvm.com/Article/details/gleyuigyh.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fehbvm.com/Article/details/gzqjefwhe.sHtML

[T14] Kotlin：循环
来源：http://baike.zdbjq.cn/Article/details/gzprzevoq.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fehbvm.com/Article/details/grcavsqnf.sHtML

[T15] Kotlin：接口
来源：http://www.blog.hesvh.cn/Article/details/ggvhfkvll.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fehbvm.com/Article/details/gwbmnbnyo.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gpcfmkiet.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/gjctglsij.sHtML

[T17] Swift：变量与常量
来源：http://baike.hesvh.cn/Article/details/gbmhtyzdg.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gswhcakyn.sHtML

[T18] Swift：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gcmruatvn.sHtML

"值: \(b)"
来源：http://www.share.hesvh.cn/Article/details/gqqpoossp.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fehbvm.com/Article/details/gvkiyirnb.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.zdbjq.cn/Article/details/gsjfuzuqs.sHtML

[T20] Swift：数组操作
来源：http://wap.fehbvm.com/Article/details/gbfvemqcg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.zdbjq.cn/Article/details/gqgawxajy.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fehbvm.com/Article/details/gxccxggdh.sHtML

for x in a { print(x) }
来源：http://www.share.zdbjq.cn/Article/details/ghauhfzsb.sHtML

[T22] Swift：字典
来源：http://www.m.share.zdbjq.cn/Article/details/gnwmpsyzi.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.zdbjq.cn/Article/details/gjewilwps.sHtML

[T23] Swift：函数
来源：http://mobile.hesvh.cn/Article/details/gzvdllgwc.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fehbvm.com/Article/details/gzovjigit.sHtML

[T24] Swift：闭包
来源：http://mobile.hesvh.cn/Article/details/ggktaeshy.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.zdbjq.cn/Article/details/gtxymcsdo.sHtML

[T25] Swift：结构体
来源：http://www.share.fehbvm.com/Article/details/gtduvhhrg.sHtML

struct P { var x: Int }
来源：http://blog.fehbvm.com/Article/details/gspwemcay.sHtML

[T26] Swift：类与重写
来源：http://wap.fehbvm.com/Article/details/gzqgbnzli.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fehbvm.com/Article/details/grrfxzbra.sHtML

[T27] Swift：错误处理
来源：http://www.share.hesvh.cn/Article/details/gzhvjhtzw.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fehbvm.com/Article/details/ggcppspda.sHtML

[T28] Swift：枚举
来源：http://blog.zdbjq.cn/Article/details/gxiighobx.sHtML

enum Color { case red, green }
来源：http://mobile.fehbvm.com/Article/details/gbkxdvwtt.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.zdbjq.cn/Article/details/gznmetudc.sHtML

guard let x = opt else { return }
来源：http://wap.fehbvm.com/Article/details/gbteoqeef.sHtML

[T30] Swift：协议
来源：http://www.m.share.fehbvm.com/Article/details/gusjbziuj.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.zdbjq.cn/Article/details/gtocvysjr.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gqovrqdnr.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/gwlraucep.sHtML

[T32] Lua：局部变量
来源：http://www.blog.zdbjq.cn/Article/details/greojfyib.sHtML

local a = 1
来源：http://www.blog.zdbjq.cn/Article/details/ghsyraygw.sHtML

[T33] Lua：表（数组）
来源：http://read.share.hesvh.cn/Article/details/godjrvxop.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fehbvm.com/Article/details/gaapcdzos.sHtML

[T34] Lua：遍历表
来源：http://www.blog.hesvh.cn/Article/details/gtwgjweit.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.fehbvm.com/Article/details/gkpcuezpz.sHtML


<!-- 参考信息 -->