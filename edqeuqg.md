代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fehbvm.com/Article/details/glhwghohj.sHtML

[R36] 并发执行多个任务
来源：http://3g.fehbvm.com/Article/details/gktdgrpjq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.zdbjq.cn/Article/details/gaubthfci.sHtML

[R37] 把输出赋给变量
来源：http://blog.zdbjq.cn/Article/details/gbvwsxkbd.sHtML

files=$(ls -1)
来源：http://baike.fehbvm.com/Article/details/genelebli.sHtML

[R38] 管道串联
来源：http://blog.zdbjq.cn/Article/details/gqtlohgzx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.zdbjq.cn/Article/details/gfrscmbde.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.zdbjq.cn/Article/details/gkvlfabmf.sHtML

cmd > out.log 2>&1
来源：http://wap.zdbjq.cn/Article/details/gywpqsneb.sHtML

[R40] 追加写日志
来源：http://www.m.share.fehbvm.com/Article/details/glhyclxgf.sHtML

echo "log" >> out.log
来源：http://baike.zdbjq.cn/Article/details/gxkehoaby.sHtML

[R41] 丢弃输出
来源：http://www.share.zdbjq.cn/Article/details/gvwozevan.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fehbvm.com/Article/details/gosrkvtfd.sHtML

[R42] 输入重定向
来源：http://m.share.zdbjq.cn/Article/details/gkzzefsgd.sHtML

wc -l < a.txt
来源：http://wap.hesvh.cn/Article/details/gfrjfdspl.sHtML

[R43] 按名字查找文件
来源：http://www.share.zdbjq.cn/Article/details/grljkqlyf.sHtML

find . -name "*.log" -type f
来源：http://blog.fehbvm.com/Article/details/ginpdqxte.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.hesvh.cn/Article/details/gpfzahaoi.sHtML

find . -mtime -7 -type f
来源：http://m.share.hesvh.cn/Article/details/gtvpjazkk.sHtML

[R45] 批量删除
来源：http://www.blog.fehbvm.com/Article/details/gbpqhlysu.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fehbvm.com/Article/details/gaiouwshv.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fehbvm.com/Article/details/gzrywhowv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.hesvh.cn/Article/details/gouylkhjw.sHtML

[R47] sed 单行替换
来源：http://read.share.fehbvm.com/Article/details/gcysczqen.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gyqvllwna.sHtML

[R48] awk 取指定列
来源：http://www.blog.fehbvm.com/Article/details/gktdnrssm.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gmfkblizf.sHtML

[R49] awk 带条件
来源：http://mobile.hesvh.cn/Article/details/geeriytcg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.zdbjq.cn/Article/details/gksckarsd.sHtML

[R50] awk 求和
来源：http://3g.fehbvm.com/Article/details/gfdqqpzbs.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.hesvh.cn/Article/details/gvpzllsev.sHtML

[R51] 排序去重取前几
来源：http://3g.hesvh.cn/Article/details/gzsrxoamw.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.zdbjq.cn/Article/details/ghtqbwzuj.sHtML

[R52] 统计行数
来源：http://m.share.zdbjq.cn/Article/details/ghjklqegd.sHtML

wc -l a.txt
来源：http://read.share.zdbjq.cn/Article/details/gcixfmigb.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.zdbjq.cn/Article/details/gbthzfzgd.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.hesvh.cn/Article/details/grilzygyj.sHtML

[R54] 比较两个文件
来源：http://blog.zdbjq.cn/Article/details/gualjqgnc.sHtML

diff a.txt b.txt
来源：http://www.blog.zdbjq.cn/Article/details/gymuvzruq.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fehbvm.com/Article/details/gzgnzcpjo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fehbvm.com/Article/details/gubugcatn.sHtML

[R56] 远程拷贝
来源：http://mobile.fehbvm.com/Article/details/gwocchevb.sHtML

scp file user@host:/path/
来源：http://3g.zdbjq.cn/Article/details/gzvsdcytp.sHtML

[R57] 远程执行命令
来源：http://wap.fehbvm.com/Article/details/gztkvnjhi.sHtML

ssh user@host 'uptime'
来源：http://blog.zdbjq.cn/Article/details/gkvfsppck.sHtML

[R58] 下载文件
来源：http://read.share.zdbjq.cn/Article/details/glpxfkjbf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fehbvm.com/Article/details/gaxgctmoe.sHtML

[R59] 发 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/gysyewzyp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.zdbjq.cn/Article/details/gdtmzzjaf.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/gkrcyfgin.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.hesvh.cn/Article/details/gzpqxbqqf.sHtML

[R61] 磁盘占用
来源：http://m.share.zdbjq.cn/Article/details/grzrhuqor.sHtML

df -h;  du -sh *
来源：http://read.share.fehbvm.com/Article/details/gvgscwpnp.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.zdbjq.cn/Article/details/gwxasvpjy.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.zdbjq.cn/Article/details/gqzgiukvm.sHtML

[R63] 内存与进程
来源：http://www.share.fehbvm.com/Article/details/gdfqypfot.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.zdbjq.cn/Article/details/gpiumqcyi.sHtML

[R64] 结束进程
来源：http://www.m.share.zdbjq.cn/Article/details/gplfnxoic.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.hesvh.cn/Article/details/gpxkmggvw.sHtML

[R65] 查看端口占用
来源：http://m.share.fehbvm.com/Article/details/gpumbungo.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.zdbjq.cn/Article/details/geejispbl.sHtML

[R66] 定时任务
来源：http://read.share.zdbjq.cn/Article/details/grkwynler.sHtML

crontab -e;  crontab -l
来源：http://baike.fehbvm.com/Article/details/gdhifbzzm.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.hesvh.cn/Article/details/gpomrvwvi.sHtML

openssl rand -hex 16
来源：http://www.blog.hesvh.cn/Article/details/glydjaoev.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fehbvm.com/Article/details/grqaljijy.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.zdbjq.cn/Article/details/gowtyvdnk.sHtML

[R69] 生成随机密码
来源：http://baike.zdbjq.cn/Article/details/gjzqsvjtq.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.hesvh.cn/Article/details/gwbuwztws.sHtML

[R70] 时间戳与互转
来源：http://m.share.fehbvm.com/Article/details/gkysjzaqu.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.hesvh.cn/Article/details/gjlffdlaj.sHtML

[R71] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/gvuojupnv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fehbvm.com/Article/details/gxasmjrqf.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.zdbjq.cn/Article/details/gcqjfcxeu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/ggzfsxmkg.sHtML

[R73] 分割大日志
来源：http://3g.fehbvm.com/Article/details/gfiokqbor.sHtML

split -l 1000 big.log part_
来源：http://read.share.zdbjq.cn/Article/details/gzgswivxc.sHtML

[R74] 批量重命名
来源：http://www.blog.fehbvm.com/Article/details/gwwkzlxzs.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.hesvh.cn/Article/details/gqegdeene.sHtML

[R75] 导出环境变量
来源：http://wap.fehbvm.com/Article/details/guyqrxbok.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.hesvh.cn/Article/details/gccuqjtop.sHtML

[R76] 使用临时文件
来源：http://wap.hesvh.cn/Article/details/gvaeladux.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/gjonvhrkm.sHtML

[R77] 读取用户输入
来源：http://baike.fehbvm.com/Article/details/gxzajqzye.sHtML

read -rp "请输入: " ans
来源：http://wap.fehbvm.com/Article/details/gamxepoud.sHtML

[R78] 交互式菜单
来源：http://www.share.hesvh.cn/Article/details/gdveljyvn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.zdbjq.cn/Article/details/gfbivnbas.sHtML

[R79] 解析命令行选项
来源：http://www.share.hesvh.cn/Article/details/gqmcehojh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fehbvm.com/Article/details/gdiafzoon.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.zdbjq.cn/Article/details/gclirxgpq.sHtML

time ./run.sh
来源：http://www.blog.hesvh.cn/Article/details/gncyqurjg.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ggwrjuxxe.sHtML

S. C / C++ 专题
来源：http://wap.zdbjq.cn/Article/details/gebrfbbms.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gjkbyoleo.sHtML

[S01] C：Hello World
来源：http://www.share.fehbvm.com/Article/details/ghetycdmt.sHtML

#include <stdio.h>
来源：http://www.share.hesvh.cn/Article/details/ggnhjcnkg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.hesvh.cn/Article/details/gyivvodom.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fehbvm.com/Article/details/gtpwxkpkd.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.hesvh.cn/Article/details/garwipxyb.sHtML

[S03] C：读入整数
来源：http://www.m.share.fehbvm.com/Article/details/gwcgzuolp.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fehbvm.com/Article/details/gaxgqdxju.sHtML

[S04] C：字符串复制
来源：http://baike.hesvh.cn/Article/details/gibsbsqkh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fehbvm.com/Article/details/gbvxdqiix.sHtML

[S05] C：字符串长度
来源：http://3g.fehbvm.com/Article/details/gocbjnqtp.sHtML

strlen(s)
来源：http://www.blog.zdbjq.cn/Article/details/gxjqgooyg.sHtML

[S06] C：字符串比较
来源：http://blog.fehbvm.com/Article/details/gblawulog.sHtML

strcmp(a, b) == 0
来源：http://read.share.hesvh.cn/Article/details/gtjxhmdnf.sHtML

[S07] C：数组遍历求和
来源：http://blog.zdbjq.cn/Article/details/grruhhxom.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.zdbjq.cn/Article/details/gxbvxnypw.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.zdbjq.cn/Article/details/gaevqyndx.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fehbvm.com/Article/details/gblpfipmh.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fehbvm.com/Article/details/gjngnyibr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fehbvm.com/Article/details/ggqjauwee.sHtML

[S10] C：指针与解引用
来源：http://wap.fehbvm.com/Article/details/grymdfjup.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fehbvm.com/Article/details/godxwufzw.sHtML

[S11] C：逐行读文件
来源：http://3g.hesvh.cn/Article/details/giiqsbomf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.hesvh.cn/Article/details/guuoiqdny.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.hesvh.cn/Article/details/gvuzgitje.sHtML

fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/glavtjzxh.sHtML

[S12] C：写文件
来源：http://3g.fehbvm.com/Article/details/gptbvktbq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.zdbjq.cn/Article/details/gkgvmkwvf.sHtML

[S13] C：宏定义
来源：http://www.blog.zdbjq.cn/Article/details/gefopgaan.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.zdbjq.cn/Article/details/gptjewgfe.sHtML

[S14] C：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gwlorzuze.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fehbvm.com/Article/details/gkargknev.sHtML

[S15] C：类型转换
来源：http://m.share.zdbjq.cn/Article/details/godnicrbq.sHtML

(double) a / b
来源：http://www.share.hesvh.cn/Article/details/gqzlevxcj.sHtML

[S16] C：位操作置位
来源：http://blog.fehbvm.com/Article/details/gwpnbwjta.sHtML

x |= (1 << 3);
来源：http://mobile.fehbvm.com/Article/details/gppmiqzpb.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gqbwxeuaz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.zdbjq.cn/Article/details/goytmkkym.sHtML

[S18] C：命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/gcwwaescz.sHtML

int main(int argc, char **argv)
来源：http://3g.hesvh.cn/Article/details/gpncykuus.sHtML

[S19] C：快速排序
来源：http://www.blog.hesvh.cn/Article/details/ghawzopny.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/gjefhntzr.sHtML

[S20] C：二分查找
来源：http://read.share.hesvh.cn/Article/details/guiziwldr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/gxhxfdfio.sHtML

[S21] C：字符类别判断
来源：http://m.share.hesvh.cn/Article/details/gihuquxwj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.zdbjq.cn/Article/details/gsegprlle.sHtML

[S22] C：字符串转数字
来源：http://3g.zdbjq.cn/Article/details/guuqpsmcq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fehbvm.com/Article/details/gcozfqlol.sHtML

[S23] C：随机数
来源：http://read.share.zdbjq.cn/Article/details/gsqkbbiwn.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.hesvh.cn/Article/details/gmhbwqhrv.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fehbvm.com/Article/details/gntnpqijw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.zdbjq.cn/Article/details/gnepvwrhq.sHtML

[S25] C：内存拷贝
来源：http://baike.hesvh.cn/Article/details/garxdihcc.sHtML

memcpy(dst, src, n);
来源：http://3g.zdbjq.cn/Article/details/gdflcixqk.sHtML

[S26] C：内存清零
来源：http://wap.zdbjq.cn/Article/details/gmjamdxzs.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fehbvm.com/Article/details/guuwzkwah.sHtML

[S27] C：定义常量
来源：http://m.share.hesvh.cn/Article/details/gaqjyhaio.sHtML

const double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gtkdawffn.sHtML

[S28] C：静态变量
来源：http://baike.hesvh.cn/Article/details/glkdnclxt.sHtML

static int counter = 0;
来源：http://www.m.share.fehbvm.com/Article/details/gjrqsgvux.sHtML

[S29] C：变参函数
来源：http://www.blog.zdbjq.cn/Article/details/ghdjagiyt.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fehbvm.com/Article/details/gxmsxvbjd.sHtML

[S30] C：头文件保护
来源：http://blog.hesvh.cn/Article/details/ghwohzegg.sHtML

#ifndef X_H
来源：http://m.share.hesvh.cn/Article/details/gumupdojr.sHtML

#define X_H
来源：http://wap.hesvh.cn/Article/details/gemzvhyxf.sHtML

#endif
来源：http://www.blog.fehbvm.com/Article/details/gixzgabsf.sHtML

[S31] C++：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gljazfdra.sHtML

#include <iostream>
来源：http://blog.fehbvm.com/Article/details/gnguhuckn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fehbvm.com/Article/details/gujbrjwkb.sHtML

[S32] C++：字符串
来源：http://baike.zdbjq.cn/Article/details/geejugefv.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.zdbjq.cn/Article/details/gsrezzfgl.sHtML

[S33] C++：vector 增删
来源：http://baike.zdbjq.cn/Article/details/gzvqxrlmf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gbekygjqs.sHtML

[S34] C++：遍历 vector
来源：http://blog.hesvh.cn/Article/details/guljkhjpp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.hesvh.cn/Article/details/gudydette.sHtML

[S35] C++：map
来源：http://m.share.fehbvm.com/Article/details/gnkwkfofg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/ggntarofx.sHtML

[S36] C++：unordered_map
来源：http://mobile.hesvh.cn/Article/details/gsahefsyo.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gpcvcavsj.sHtML

[S37] C++：set
来源：http://mobile.fehbvm.com/Article/details/gctnxwfaw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.zdbjq.cn/Article/details/ganrswceg.sHtML

[S38] C++：排序
来源：http://www.m.share.zdbjq.cn/Article/details/gjlizwbyi.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fehbvm.com/Article/details/gsistdwyc.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fehbvm.com/Article/details/ggtoogewe.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.hesvh.cn/Article/details/gwgnannsg.sHtML

[S40] C++：查找元素
来源：http://wap.hesvh.cn/Article/details/gdpwzzmbl.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fehbvm.com/Article/details/gqhhuxvog.sHtML

[S41] C++：类与构造函数
来源：http://blog.hesvh.cn/Article/details/ggfsoicdj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fehbvm.com/Article/details/gylvfecul.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.hesvh.cn/Article/details/gkilwzahh.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.hesvh.cn/Article/details/glxtmujyv.sHtML

[S43] C++：智能指针
来源：http://baike.hesvh.cn/Article/details/gfqptdxjd.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.zdbjq.cn/Article/details/gfzllvjlu.sHtML

[S44] C++：引用传参
来源：http://www.share.fehbvm.com/Article/details/gmomjpedh.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fehbvm.com/Article/details/ggcflvnwp.sHtML

[S45] C++：lambda
来源：http://3g.fehbvm.com/Article/details/gygcdljoo.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fehbvm.com/Article/details/gzzxxzvbn.sHtML

[S46] C++：函数模板
来源：http://www.m.share.hesvh.cn/Article/details/gffmmxfwz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.hesvh.cn/Article/details/gsyqtejzu.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.zdbjq.cn/Article/details/gaoiktsbl.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.hesvh.cn/Article/details/gdicvsysj.sHtML

[S48] C++：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gtjmbqvvs.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.hesvh.cn/Article/details/gqecpiilp.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fehbvm.com/Article/details/gpiammsdh.sHtML

[S49] C++：写文件
来源：http://wap.zdbjq.cn/Article/details/gqpvrcqng.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.hesvh.cn/Article/details/gfczgkmoe.sHtML

[S50] C++：格式化数字
来源：http://www.blog.zdbjq.cn/Article/details/glmimjngu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gkxeriocu.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fehbvm.com/Article/details/gdklyvzuw.sHtML

static_cast<double>(a) / b
来源：http://www.share.fehbvm.com/Article/details/girsxvsro.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fehbvm.com/Article/details/gcbxeeidw.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fehbvm.com/Article/details/gqplcvoqo.sHtML

[S53] C++：移动语义
来源：http://3g.hesvh.cn/Article/details/gkqifvqjh.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.zdbjq.cn/Article/details/gaabgdweq.sHtML

[S54] C++：异常处理
来源：http://m.share.zdbjq.cn/Article/details/gwzdmrqwk.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.hesvh.cn/Article/details/gftsfuypp.sHtML

[S55] C++：结构化绑定
来源：http://mobile.zdbjq.cn/Article/details/glxsxlitt.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.zdbjq.cn/Article/details/gjolynpax.sHtML

[S56] C++：optional
来源：http://baike.fehbvm.com/Article/details/gtwrlpqlr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fehbvm.com/Article/details/gvivvzmol.sHtML

[S57] C++：编译期常量
来源：http://www.share.zdbjq.cn/Article/details/gtxboasnx.sHtML

constexpr int N = 10;
来源：http://mobile.zdbjq.cn/Article/details/gorlpwufx.sHtML

[S58] C++：命名空间
来源：http://www.m.share.hesvh.cn/Article/details/gsznonaau.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.zdbjq.cn/Article/details/gjhnagagx.sHtML

[S59] C++：静态断言
来源：http://www.m.share.hesvh.cn/Article/details/gkpjjgadu.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.hesvh.cn/Article/details/gmjxyutwo.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.hesvh.cn/Article/details/gxylkejhn.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fehbvm.com/Article/details/gwpihqtkz.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gwezbbxpc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.hesvh.cn/Article/details/ggtssvbaj.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gfhhfrtcf.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.hesvh.cn/Article/details/gaoxldqez.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gcyypdxhu.sHtML

[T02] Kotlin：变量
来源：http://baike.fehbvm.com/Article/details/glqgorapw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.zdbjq.cn/Article/details/gutwpfhjn.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.hesvh.cn/Article/details/gcghboopa.sHtML

"值: $b"
来源：http://www.share.hesvh.cn/Article/details/gleqcuqeh.sHtML

[T04] Kotlin：空安全
来源：http://mobile.hesvh.cn/Article/details/gqgvaikhy.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fehbvm.com/Article/details/gebmjdbhx.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fehbvm.com/Article/details/gxbgsomoe.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.hesvh.cn/Article/details/gsefztlgo.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.hesvh.cn/Article/details/gfmpumpfy.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.hesvh.cn/Article/details/gbedmvmmo.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.hesvh.cn/Article/details/gxqxnejss.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.zdbjq.cn/Article/details/gjutfbjqr.sHtML

[T08] Kotlin：数据类
来源：http://read.share.zdbjq.cn/Article/details/gxjgitwec.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/gxcnlnonq.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fehbvm.com/Article/details/gbmgksxjx.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.zdbjq.cn/Article/details/gfzbuouob.sHtML

[T10] Kotlin：默认参数
来源：http://baike.zdbjq.cn/Article/details/gqnhecvrk.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fehbvm.com/Article/details/glhewriug.sHtML

[T11] Kotlin：协程
来源：http://mobile.hesvh.cn/Article/details/gzciewajy.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.zdbjq.cn/Article/details/gacsgyupr.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.zdbjq.cn/Article/details/gnlmxshhy.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gedxqlgkc.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.zdbjq.cn/Article/details/glihyqwrf.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fehbvm.com/Article/details/gnrcqeppp.sHtML

[T14] Kotlin：循环
来源：http://baike.hesvh.cn/Article/details/gnaypqhpu.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fehbvm.com/Article/details/grysxbuhc.sHtML

[T15] Kotlin：接口
来源：http://blog.fehbvm.com/Article/details/gxgcadpfo.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fehbvm.com/Article/details/gybzptivb.sHtML

[T16] Swift：Hello World
来源：http://wap.hesvh.cn/Article/details/gfodsutnc.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/gotwkslvd.sHtML

[T17] Swift：变量与常量
来源：http://3g.fehbvm.com/Article/details/gdcbooyqd.sHtML

var a = 1;  let b = 2
来源：http://3g.zdbjq.cn/Article/details/gdnanarve.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gjeisezaa.sHtML

"值: \(b)"
来源：http://www.share.zdbjq.cn/Article/details/gemhufpvn.sHtML

[T19] Swift：可选绑定
来源：http://3g.hesvh.cn/Article/details/glppjrhev.sHtML

if let n = opt { print(n) }
来源：http://mobile.zdbjq.cn/Article/details/gjquolsam.sHtML

[T20] Swift：数组操作
来源：http://3g.hesvh.cn/Article/details/gpxdwpmdt.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.hesvh.cn/Article/details/gwwnosygn.sHtML

[T21] Swift：遍历
来源：http://3g.fehbvm.com/Article/details/gravptcej.sHtML

for x in a { print(x) }
来源：http://www.m.share.fehbvm.com/Article/details/gsxsgzyhq.sHtML

[T22] Swift：字典
来源：http://www.blog.hesvh.cn/Article/details/ggfbxgumk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.hesvh.cn/Article/details/geyentagx.sHtML

[T23] Swift：函数
来源：http://read.share.zdbjq.cn/Article/details/gxtwehwzg.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.zdbjq.cn/Article/details/gvpfdibun.sHtML

[T24] Swift：闭包
来源：http://blog.zdbjq.cn/Article/details/gzqhfcrlk.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fehbvm.com/Article/details/gwsrifcvo.sHtML

[T25] Swift：结构体
来源：http://3g.zdbjq.cn/Article/details/gsshdvhsg.sHtML

struct P { var x: Int }
来源：http://3g.hesvh.cn/Article/details/gasfcrvda.sHtML

[T26] Swift：类与重写
来源：http://wap.zdbjq.cn/Article/details/ghrzzdnhg.sHtML

class A: Base { override func f() {} }
来源：http://read.share.zdbjq.cn/Article/details/gtolxxmnb.sHtML

[T27] Swift：错误处理
来源：http://www.blog.hesvh.cn/Article/details/gowzbddwl.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.zdbjq.cn/Article/details/gsqfniquo.sHtML

[T28] Swift：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gbxzjlqum.sHtML

enum Color { case red, green }
来源：http://blog.zdbjq.cn/Article/details/ghydejwzu.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.zdbjq.cn/Article/details/gcvozssaa.sHtML

guard let x = opt else { return }
来源：http://mobile.fehbvm.com/Article/details/gwmetoosu.sHtML

[T30] Swift：协议
来源：http://www.blog.zdbjq.cn/Article/details/gnumrzljc.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fehbvm.com/Article/details/gyljnjgbi.sHtML

[T31] Lua：Hello World
来源：http://www.share.fehbvm.com/Article/details/gkdrvrqyb.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/ganoadess.sHtML

[T32] Lua：局部变量
来源：http://wap.zdbjq.cn/Article/details/gcdvqlaet.sHtML

local a = 1
来源：http://www.blog.fehbvm.com/Article/details/guzblxocw.sHtML

[T33] Lua：表（数组）
来源：http://blog.zdbjq.cn/Article/details/gdfseqyha.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.hesvh.cn/Article/details/gifjdknmu.sHtML

[T34] Lua：遍历表
来源：http://m.share.zdbjq.cn/Article/details/gsqusglpv.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.zdbjq.cn/Article/details/gpemzclbx.sHtML

[T35] Lua：字典表
来源：http://wap.zdbjq.cn/Article/details/gwwyswqmf.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.fehbvm.com/Article/details/gpftoixgi.sHtML

[T36] Lua：函数
来源：http://3g.zdbjq.cn/Article/details/gdqklpdez.sHtML

function add(a, b) return a + b end
来源：http://m.share.hesvh.cn/Article/details/geowyfzby.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/gpvroohzn.sHtML

"a" .. "b"
来源：http://m.share.fehbvm.com/Article/details/glursfqem.sHtML

[T38] Lua：条件
来源：http://3g.fehbvm.com/Article/details/gonzursvq.sHtML

if x > 0 then print("正") end
来源：http://m.share.zdbjq.cn/Article/details/gucnhwawp.sHtML


<!-- 参考信息 -->