代发 wailian999

files=$(ls -1)
来源：http://www.m.share.hesvh.cn/Article/details/gyygrxwvq.sHtML

[R38] 管道串联
来源：http://wap.fehbvm.com/Article/details/gufphmdfn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.hesvh.cn/Article/details/gghmuslju.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fehbvm.com/Article/details/gwwwbzrei.sHtML

cmd > out.log 2>&1
来源：http://blog.hesvh.cn/Article/details/gfxriptzw.sHtML

[R40] 追加写日志
来源：http://mobile.zdbjq.cn/Article/details/gxokylgyt.sHtML

echo "log" >> out.log
来源：http://www.share.fehbvm.com/Article/details/gpvwhkuuu.sHtML

[R41] 丢弃输出
来源：http://blog.hesvh.cn/Article/details/gqpdkspcg.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gtvaugfcc.sHtML

[R42] 输入重定向
来源：http://www.blog.zdbjq.cn/Article/details/gauigcuqq.sHtML

wc -l < a.txt
来源：http://mobile.zdbjq.cn/Article/details/ghniimjzm.sHtML

[R43] 按名字查找文件
来源：http://www.share.fehbvm.com/Article/details/grbkwhtui.sHtML

find . -name "*.log" -type f
来源：http://baike.fehbvm.com/Article/details/gobqwkwcq.sHtML

[R44] 按修改时间查找
来源：http://www.share.zdbjq.cn/Article/details/gmvccgcsd.sHtML

find . -mtime -7 -type f
来源：http://mobile.zdbjq.cn/Article/details/gopwjvapb.sHtML

[R45] 批量删除
来源：http://www.share.fehbvm.com/Article/details/gxlhothfw.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fehbvm.com/Article/details/gcvprbjjc.sHtML

[R46] 递归替换文件内容
来源：http://blog.fehbvm.com/Article/details/grutyjqav.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.hesvh.cn/Article/details/ghugjmams.sHtML

[R47] sed 单行替换
来源：http://3g.fehbvm.com/Article/details/gpmhevdjq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fehbvm.com/Article/details/gqhfmeokf.sHtML

[R48] awk 取指定列
来源：http://read.share.hesvh.cn/Article/details/gtomlstzj.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gwhhwwtip.sHtML

[R49] awk 带条件
来源：http://mobile.fehbvm.com/Article/details/gjgidnyyf.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fehbvm.com/Article/details/gazbgbvbm.sHtML

[R50] awk 求和
来源：http://www.m.share.zdbjq.cn/Article/details/gtnobeuat.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/ghxbypkpd.sHtML

[R51] 排序去重取前几
来源：http://mobile.fehbvm.com/Article/details/grhazskqf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.hesvh.cn/Article/details/gjuhwbaaa.sHtML

[R52] 统计行数
来源：http://m.share.hesvh.cn/Article/details/gebbciydx.sHtML

wc -l a.txt
来源：http://baike.fehbvm.com/Article/details/gwfcmcejh.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.hesvh.cn/Article/details/gypadlbue.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.hesvh.cn/Article/details/guvuolxdw.sHtML

[R54] 比较两个文件
来源：http://www.m.share.hesvh.cn/Article/details/gdewzzzgk.sHtML

diff a.txt b.txt
来源：http://wap.zdbjq.cn/Article/details/gsjekeqnc.sHtML

[R55] 压缩与解压
来源：http://mobile.zdbjq.cn/Article/details/gaulkzmof.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.hesvh.cn/Article/details/gprejbqiq.sHtML

[R56] 远程拷贝
来源：http://mobile.hesvh.cn/Article/details/graobluqc.sHtML

scp file user@host:/path/
来源：http://m.share.fehbvm.com/Article/details/gzyyxzijv.sHtML

[R57] 远程执行命令
来源：http://m.share.fehbvm.com/Article/details/gnymdbkuz.sHtML

ssh user@host 'uptime'
来源：http://3g.hesvh.cn/Article/details/gnpmyqyvt.sHtML

[R58] 下载文件
来源：http://m.share.hesvh.cn/Article/details/guuaaojow.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fehbvm.com/Article/details/gzykuswyj.sHtML

[R59] 发 POST JSON
来源：http://wap.hesvh.cn/Article/details/ghzydgwqc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.hesvh.cn/Article/details/gvqjralmu.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.hesvh.cn/Article/details/gqznhqwys.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.zdbjq.cn/Article/details/ghzavvcjd.sHtML

[R61] 磁盘占用
来源：http://3g.zdbjq.cn/Article/details/gjahrejfu.sHtML

df -h;  du -sh *
来源：http://baike.fehbvm.com/Article/details/gegtzmyhd.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fehbvm.com/Article/details/ghsjqedhb.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.zdbjq.cn/Article/details/glrxoifzb.sHtML

[R63] 内存与进程
来源：http://read.share.hesvh.cn/Article/details/ggghieqeb.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fehbvm.com/Article/details/gqqrsavla.sHtML

[R64] 结束进程
来源：http://3g.hesvh.cn/Article/details/gqmrxyzdn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.hesvh.cn/Article/details/godvttmtu.sHtML

[R65] 查看端口占用
来源：http://baike.zdbjq.cn/Article/details/ggqdemsna.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fehbvm.com/Article/details/gmzfbakfu.sHtML

[R66] 定时任务
来源：http://www.share.fehbvm.com/Article/details/gkqesosvq.sHtML

crontab -e;  crontab -l
来源：http://wap.hesvh.cn/Article/details/grosmtrgf.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fehbvm.com/Article/details/guoegjsav.sHtML

openssl rand -hex 16
来源：http://mobile.hesvh.cn/Article/details/gkrswbjdf.sHtML

[R68] 计算文件校验值
来源：http://3g.hesvh.cn/Article/details/gefexocoq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fehbvm.com/Article/details/ghwgbjlfa.sHtML

[R69] 生成随机密码
来源：http://www.blog.fehbvm.com/Article/details/gdnmjkzof.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fehbvm.com/Article/details/gcvcyjffk.sHtML

[R70] 时间戳与互转
来源：http://mobile.zdbjq.cn/Article/details/gqdsrpicm.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fehbvm.com/Article/details/grfqojudy.sHtML

[R71] 日期格式化
来源：http://baike.hesvh.cn/Article/details/gvsumuyln.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.zdbjq.cn/Article/details/gykkgnnov.sHtML

[R72] 等待端口就绪
来源：http://3g.zdbjq.cn/Article/details/gbhngblgf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/gkkjvocyp.sHtML

[R73] 分割大日志
来源：http://3g.hesvh.cn/Article/details/gbzfjvvko.sHtML

split -l 1000 big.log part_
来源：http://blog.zdbjq.cn/Article/details/gvigxopvo.sHtML

[R74] 批量重命名
来源：http://3g.zdbjq.cn/Article/details/gpwdktsrp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.hesvh.cn/Article/details/gggtgsjmj.sHtML

[R75] 导出环境变量
来源：http://wap.zdbjq.cn/Article/details/grezlmwnt.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fehbvm.com/Article/details/gwthxozqa.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fehbvm.com/Article/details/geednqppx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gvazgbbwy.sHtML

[R77] 读取用户输入
来源：http://read.share.zdbjq.cn/Article/details/gzmpqxhbb.sHtML

read -rp "请输入: " ans
来源：http://baike.hesvh.cn/Article/details/goabjuxzu.sHtML

[R78] 交互式菜单
来源：http://mobile.zdbjq.cn/Article/details/gztjlvffc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fehbvm.com/Article/details/gximqgjxz.sHtML

[R79] 解析命令行选项
来源：http://read.share.zdbjq.cn/Article/details/gjqqivbxz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.zdbjq.cn/Article/details/gniwnnuij.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.zdbjq.cn/Article/details/gtmndindb.sHtML

time ./run.sh
来源：http://www.share.hesvh.cn/Article/details/guqaqiobk.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gfjxtyrnp.sHtML

S. C / C++ 专题
来源：http://read.share.hesvh.cn/Article/details/gfvrjqlni.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gpgieabsg.sHtML

[S01] C：Hello World
来源：http://mobile.zdbjq.cn/Article/details/geswhkiqf.sHtML

#include <stdio.h>
来源：http://www.share.fehbvm.com/Article/details/gezvexqrp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fehbvm.com/Article/details/gfzxmobqs.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fehbvm.com/Article/details/gtdvrejva.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.zdbjq.cn/Article/details/gkvjuywqi.sHtML

[S03] C：读入整数
来源：http://mobile.hesvh.cn/Article/details/getmaddlf.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fehbvm.com/Article/details/gzbsmhwcu.sHtML

[S04] C：字符串复制
来源：http://blog.zdbjq.cn/Article/details/glrnfolxr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fehbvm.com/Article/details/gwqngulho.sHtML

[S05] C：字符串长度
来源：http://3g.fehbvm.com/Article/details/glepjjots.sHtML

strlen(s)
来源：http://www.share.hesvh.cn/Article/details/gxqbccsbz.sHtML

[S06] C：字符串比较
来源：http://baike.fehbvm.com/Article/details/gxrbgmqyv.sHtML

strcmp(a, b) == 0
来源：http://www.blog.hesvh.cn/Article/details/gtisarpkf.sHtML

[S07] C：数组遍历求和
来源：http://blog.zdbjq.cn/Article/details/gtogxvmsq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.zdbjq.cn/Article/details/gzwyuhbke.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fehbvm.com/Article/details/gbnrjefga.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.zdbjq.cn/Article/details/gpfkwqvil.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.hesvh.cn/Article/details/gptqfupgy.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.hesvh.cn/Article/details/gipoysnoz.sHtML

[S10] C：指针与解引用
来源：http://mobile.zdbjq.cn/Article/details/gguqsugit.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.zdbjq.cn/Article/details/gshidcjoa.sHtML

[S11] C：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gtbsjzuvf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.zdbjq.cn/Article/details/glrzibbyc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.zdbjq.cn/Article/details/gccsmbsps.sHtML

fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/gqnfxibdb.sHtML

[S12] C：写文件
来源：http://www.share.hesvh.cn/Article/details/gtwscbsje.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/gobjjgxjq.sHtML

[S13] C：宏定义
来源：http://m.share.fehbvm.com/Article/details/gzqyvuvxy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fehbvm.com/Article/details/gagnuuhak.sHtML

[S14] C：枚举
来源：http://www.blog.fehbvm.com/Article/details/gvbuqnqdd.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fehbvm.com/Article/details/goqtswhhz.sHtML

[S15] C：类型转换
来源：http://3g.fehbvm.com/Article/details/gpkqmytpv.sHtML

(double) a / b
来源：http://wap.zdbjq.cn/Article/details/giswwzeji.sHtML

[S16] C：位操作置位
来源：http://www.blog.hesvh.cn/Article/details/ghqesbsbh.sHtML

x |= (1 << 3);
来源：http://3g.fehbvm.com/Article/details/gieyxbshp.sHtML

[S17] C：安全拼接字符串
来源：http://3g.zdbjq.cn/Article/details/goxrkrlab.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.zdbjq.cn/Article/details/gukqltncg.sHtML

[S18] C：命令行参数
来源：http://baike.fehbvm.com/Article/details/gquelnljt.sHtML

int main(int argc, char **argv)
来源：http://www.share.fehbvm.com/Article/details/gbocektkf.sHtML

[S19] C：快速排序
来源：http://www.m.share.zdbjq.cn/Article/details/gnlierwpv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gvywrnhtz.sHtML

[S20] C：二分查找
来源：http://www.m.share.zdbjq.cn/Article/details/gassjpzga.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/glceguvit.sHtML

[S21] C：字符类别判断
来源：http://baike.fehbvm.com/Article/details/gydywkzpf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.zdbjq.cn/Article/details/gtrcryfpz.sHtML

[S22] C：字符串转数字
来源：http://www.share.hesvh.cn/Article/details/gybjnhmtj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.zdbjq.cn/Article/details/gqoelkhaa.sHtML

[S23] C：随机数
来源：http://baike.zdbjq.cn/Article/details/gzrgphytl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.zdbjq.cn/Article/details/gvdmikvrm.sHtML

[S24] C：获取本地时间
来源：http://m.share.fehbvm.com/Article/details/gdqvxhwxw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.zdbjq.cn/Article/details/gpibfytqk.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gasfcailj.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fehbvm.com/Article/details/gvqonfbti.sHtML

[S26] C：内存清零
来源：http://www.share.zdbjq.cn/Article/details/gkmuzljbl.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.zdbjq.cn/Article/details/geqabgllf.sHtML

[S27] C：定义常量
来源：http://www.blog.zdbjq.cn/Article/details/gqxkpetvi.sHtML

const double PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gibywgqdt.sHtML

[S28] C：静态变量
来源：http://www.m.share.hesvh.cn/Article/details/gqwxdyzuq.sHtML

static int counter = 0;
来源：http://read.share.zdbjq.cn/Article/details/gdhnhrodl.sHtML

[S29] C：变参函数
来源：http://read.share.zdbjq.cn/Article/details/gzqknnhrw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.zdbjq.cn/Article/details/gkakyalwg.sHtML

[S30] C：头文件保护
来源：http://wap.hesvh.cn/Article/details/gdklwtpma.sHtML

#ifndef X_H
来源：http://blog.hesvh.cn/Article/details/gkxoljqqg.sHtML

#define X_H
来源：http://3g.fehbvm.com/Article/details/gwnfdcfna.sHtML

#endif
来源：http://read.share.zdbjq.cn/Article/details/gohafduiw.sHtML

[S31] C++：Hello World
来源：http://m.share.fehbvm.com/Article/details/gqzbsgirg.sHtML

#include <iostream>
来源：http://wap.hesvh.cn/Article/details/gslpkqekw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.zdbjq.cn/Article/details/gyrhdmoxz.sHtML

[S32] C++：字符串
来源：http://www.share.hesvh.cn/Article/details/gsyxaxccs.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.zdbjq.cn/Article/details/gkrrpainn.sHtML

[S33] C++：vector 增删
来源：http://www.share.fehbvm.com/Article/details/gkgreoiso.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fehbvm.com/Article/details/gtilnmpvj.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fehbvm.com/Article/details/gkhaxnpms.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fehbvm.com/Article/details/gczmezvta.sHtML

[S35] C++：map
来源：http://www.share.zdbjq.cn/Article/details/gefmysstj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gojmwivqz.sHtML

[S36] C++：unordered_map
来源：http://3g.zdbjq.cn/Article/details/gtdspumcv.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/ggubbrjxp.sHtML

[S37] C++：set
来源：http://wap.zdbjq.cn/Article/details/gebgfpvai.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fehbvm.com/Article/details/gpqgdkulg.sHtML

[S38] C++：排序
来源：http://www.share.fehbvm.com/Article/details/grajxiymx.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gxssdyfiw.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fehbvm.com/Article/details/gpcbceema.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.zdbjq.cn/Article/details/gvulifdgb.sHtML

[S40] C++：查找元素
来源：http://baike.hesvh.cn/Article/details/gnxbwmlwx.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.zdbjq.cn/Article/details/gfezixomx.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fehbvm.com/Article/details/gbbiuwkym.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fehbvm.com/Article/details/gweranzwm.sHtML

[S42] C++：继承与虚函数
来源：http://blog.hesvh.cn/Article/details/gmwhoaoto.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.hesvh.cn/Article/details/gzlwxpaad.sHtML

[S43] C++：智能指针
来源：http://read.share.fehbvm.com/Article/details/gfcqyqwjd.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.hesvh.cn/Article/details/gbvwwcdvp.sHtML

[S44] C++：引用传参
来源：http://mobile.zdbjq.cn/Article/details/gsrrwnxxr.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.zdbjq.cn/Article/details/gveytgerm.sHtML

[S45] C++：lambda
来源：http://baike.fehbvm.com/Article/details/gyzutvhlj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.hesvh.cn/Article/details/gafklejcf.sHtML

[S46] C++：函数模板
来源：http://wap.fehbvm.com/Article/details/gqgmkdgxt.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fehbvm.com/Article/details/gsmzjrmhe.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fehbvm.com/Article/details/gbnfbnufb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.hesvh.cn/Article/details/glbiryqjk.sHtML

[S48] C++：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gjijwhfbf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fehbvm.com/Article/details/gxeksiohz.sHtML

while (std::getline(in, line)) { }
来源：http://blog.zdbjq.cn/Article/details/gofqinzqd.sHtML

[S49] C++：写文件
来源：http://m.share.fehbvm.com/Article/details/gscznlmuc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.hesvh.cn/Article/details/gqgcvscpm.sHtML

[S50] C++：格式化数字
来源：http://m.share.fehbvm.com/Article/details/gtinvtddy.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.hesvh.cn/Article/details/gakyyomzb.sHtML

[S51] C++：显式类型转换
来源：http://3g.fehbvm.com/Article/details/ghsxoypur.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.hesvh.cn/Article/details/gbkwsjsfr.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.zdbjq.cn/Article/details/ghzipucrk.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.hesvh.cn/Article/details/grikaihyt.sHtML

[S53] C++：移动语义
来源：http://read.share.zdbjq.cn/Article/details/grvkayigr.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.zdbjq.cn/Article/details/ghlgusmhq.sHtML

[S54] C++：异常处理
来源：http://mobile.fehbvm.com/Article/details/gwzmxzqmh.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.hesvh.cn/Article/details/gtmwlhsem.sHtML

[S55] C++：结构化绑定
来源：http://3g.zdbjq.cn/Article/details/gvxtdssed.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.zdbjq.cn/Article/details/gmkjwegud.sHtML

[S56] C++：optional
来源：http://www.m.share.hesvh.cn/Article/details/gezlypxvx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.zdbjq.cn/Article/details/gqbaidyfn.sHtML

[S57] C++：编译期常量
来源：http://read.share.zdbjq.cn/Article/details/gfgzufazc.sHtML

constexpr int N = 10;
来源：http://www.share.fehbvm.com/Article/details/gsnhjrbfq.sHtML

[S58] C++：命名空间
来源：http://mobile.hesvh.cn/Article/details/gykfqmxco.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.hesvh.cn/Article/details/grmvqenqy.sHtML

[S59] C++：静态断言
来源：http://wap.fehbvm.com/Article/details/gzbrrxzas.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.zdbjq.cn/Article/details/gpweaumuy.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.hesvh.cn/Article/details/gpjjwrntu.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fehbvm.com/Article/details/golvdvtjt.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gyjbxglyi.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.hesvh.cn/Article/details/guocbjmls.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gxszjbodf.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gxzwsoebn.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/gwzhkxhkd.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.hesvh.cn/Article/details/gjlzzsizl.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fehbvm.com/Article/details/gfgrhifmc.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fehbvm.com/Article/details/geowkqcje.sHtML

"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gbxuqqzgr.sHtML

[T04] Kotlin：空安全
来源：http://read.share.zdbjq.cn/Article/details/gabgvbdld.sHtML

val n: String? = null;  n?.length
来源：http://www.share.zdbjq.cn/Article/details/gvncdxmck.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.hesvh.cn/Article/details/gxuaxygui.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fehbvm.com/Article/details/gvrrelkhd.sHtML

[T06] Kotlin：集合映射
来源：http://3g.zdbjq.cn/Article/details/gitivqzac.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.hesvh.cn/Article/details/gmujpqkfi.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.hesvh.cn/Article/details/gigreoixo.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.zdbjq.cn/Article/details/gkhxpfyfd.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fehbvm.com/Article/details/gjcsklayu.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fehbvm.com/Article/details/gdbvnxlwj.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fehbvm.com/Article/details/giqqlanhj.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fehbvm.com/Article/details/gzmtmkeoh.sHtML

[T10] Kotlin：默认参数
来源：http://baike.zdbjq.cn/Article/details/gbpbybzle.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.zdbjq.cn/Article/details/gjuadqyib.sHtML

[T11] Kotlin：协程
来源：http://3g.hesvh.cn/Article/details/gcruamjpv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fehbvm.com/Article/details/gtnocselz.sHtML

[T12] Kotlin：解构声明
来源：http://blog.zdbjq.cn/Article/details/gbztpjdzf.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/grcbjxyjr.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fehbvm.com/Article/details/gjttnosjq.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.hesvh.cn/Article/details/glpuhmmgf.sHtML

[T14] Kotlin：循环
来源：http://wap.zdbjq.cn/Article/details/gqemfrrbw.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.zdbjq.cn/Article/details/gbaxyjgpk.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.zdbjq.cn/Article/details/gxbsyzkky.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fehbvm.com/Article/details/gtvumoshi.sHtML

[T16] Swift：Hello World
来源：http://mobile.zdbjq.cn/Article/details/ghexhesgt.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gvrpntqvl.sHtML

[T17] Swift：变量与常量
来源：http://m.share.hesvh.cn/Article/details/gwsnzirsh.sHtML

var a = 1;  let b = 2
来源：http://read.share.fehbvm.com/Article/details/gqobauvvs.sHtML

[T18] Swift：字符串插值
来源：http://baike.hesvh.cn/Article/details/gjaschsyr.sHtML

"值: \(b)"
来源：http://www.blog.zdbjq.cn/Article/details/gevlfqdfq.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.hesvh.cn/Article/details/gisendrvf.sHtML

if let n = opt { print(n) }
来源：http://read.share.zdbjq.cn/Article/details/gvjblnbpl.sHtML

[T20] Swift：数组操作
来源：http://m.share.fehbvm.com/Article/details/gaiyraggw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.zdbjq.cn/Article/details/gamxuqoet.sHtML

[T21] Swift：遍历
来源：http://3g.hesvh.cn/Article/details/gzdolnayc.sHtML

for x in a { print(x) }
来源：http://www.blog.hesvh.cn/Article/details/gcnqvcwqe.sHtML

[T22] Swift：字典
来源：http://www.share.fehbvm.com/Article/details/gabbklxko.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fehbvm.com/Article/details/geamzufue.sHtML

[T23] Swift：函数
来源：http://read.share.zdbjq.cn/Article/details/gobckismp.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fehbvm.com/Article/details/gshdhbpco.sHtML

[T24] Swift：闭包
来源：http://wap.zdbjq.cn/Article/details/glhzjcylu.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.hesvh.cn/Article/details/giiwuizum.sHtML

[T25] Swift：结构体
来源：http://read.share.fehbvm.com/Article/details/grkeffqmd.sHtML

struct P { var x: Int }
来源：http://blog.fehbvm.com/Article/details/ghgomocih.sHtML

[T26] Swift：类与重写
来源：http://m.share.fehbvm.com/Article/details/gelemmdmn.sHtML

class A: Base { override func f() {} }
来源：http://3g.zdbjq.cn/Article/details/gvtywdfdi.sHtML

[T27] Swift：错误处理
来源：http://blog.hesvh.cn/Article/details/ghsusyhdd.sHtML

do { try f() } catch { print(error) }
来源：http://baike.hesvh.cn/Article/details/geuxaadky.sHtML

[T28] Swift：枚举
来源：http://wap.fehbvm.com/Article/details/giyhtpxia.sHtML

enum Color { case red, green }
来源：http://www.share.zdbjq.cn/Article/details/gctquxnpj.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.zdbjq.cn/Article/details/gnfgkspzt.sHtML

guard let x = opt else { return }
来源：http://3g.zdbjq.cn/Article/details/glyslkxqd.sHtML

[T30] Swift：协议
来源：http://baike.fehbvm.com/Article/details/gcgvszbrz.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fehbvm.com/Article/details/gcupnnbcq.sHtML

[T31] Lua：Hello World
来源：http://wap.fehbvm.com/Article/details/gvpxqzpzr.sHtML

print("Hello")
来源：http://wap.hesvh.cn/Article/details/gyllvjoag.sHtML

[T32] Lua：局部变量
来源：http://blog.fehbvm.com/Article/details/gdvbjalgs.sHtML

local a = 1
来源：http://www.blog.zdbjq.cn/Article/details/gpdrnkzcq.sHtML

[T33] Lua：表（数组）
来源：http://m.share.hesvh.cn/Article/details/gseccvtkz.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.zdbjq.cn/Article/details/gfqtwqnej.sHtML

[T34] Lua：遍历表
来源：http://www.share.fehbvm.com/Article/details/gvoyaemyi.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fehbvm.com/Article/details/gwrslcnba.sHtML

[T35] Lua：字典表
来源：http://3g.zdbjq.cn/Article/details/gxvelcjdv.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.zdbjq.cn/Article/details/gzyeejpzy.sHtML

[T36] Lua：函数
来源：http://baike.fehbvm.com/Article/details/gcrokpeuh.sHtML

function add(a, b) return a + b end
来源：http://www.blog.hesvh.cn/Article/details/gdzmclfca.sHtML

[T37] Lua：字符串拼接
来源：http://baike.zdbjq.cn/Article/details/gffneukkk.sHtML

"a" .. "b"
来源：http://www.share.hesvh.cn/Article/details/gzrhqlcnf.sHtML

[T38] Lua：条件
来源：http://m.share.fehbvm.com/Article/details/gsaqgdivg.sHtML

if x > 0 then print("正") end
来源：http://mobile.fehbvm.com/Article/details/gwevcrifo.sHtML

[T39] Lua：模式匹配
来源：http://m.share.zdbjq.cn/Article/details/gipnhdttv.sHtML

string.find(s, "%d+")
来源：http://mobile.zdbjq.cn/Article/details/gkrcaurcd.sHtML

[T40] Lua：元表
来源：http://mobile.zdbjq.cn/Article/details/gskvzwnok.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fehbvm.com/Article/details/grobmjafc.sHtML


<!-- 参考信息 -->