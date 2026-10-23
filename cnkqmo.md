代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3fwxfvftc.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3scoakxlk.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3nqimthbd.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3uvedqtog.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3wexzjqma.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3edwgscmu.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3kjcairzz.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3hwlzixpf.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3lntpssdr.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3irrifjwg.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3ayqgpcfs.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3xawjihgi.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3jhkkiraj.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3rhmtnpir.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3wgchnaub.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3naxxueej.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3ievjlsgg.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3hcdkdpen.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3egllektg.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3sfcvrryt.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3hujkryyy.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3wkgqrthg.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3rgbwvhka.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3gfphuyrl.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3kdnqbdsw.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3kvybdiuk.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3nctnhnma.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3jgrgmzhf.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3aqqmwvpj.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3bleqegoy.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3vvbpvouz.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3edyxkavd.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3rygpzzbf.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3oekwlmjr.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mswkydgs.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3aowggetf.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3dkxyjzag.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3ladpsahk.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3gjhotgmn.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3zixzwfqk.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3jokvwwfy.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3lexriodl.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3nmfpkxdu.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3mwrdeoct.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3vdenlfip.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3afhejfyb.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3zznceubj.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3dxublsuy.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3stidjnmk.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3noqgwhrg.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3hsmobbfv.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3kiwdskyi.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3wvhyvfij.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3wpfclpqn.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3caxswshr.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3midwgjnd.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3gxqkcpku.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3snhzeqrz.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3bwxlxsbz.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3vymqrral.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3favhblmz.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3bnewepfj.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3tqttirkp.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3dtzcbdyd.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3qjidarex.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3lzbvhbff.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3ovvcnsyq.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3mwdgjfym.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3icqsplew.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3sryorvxy.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3kogewpdg.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3ttfafbpb.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3hazlgkhn.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3jtdcpfqn.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3mzcudgqg.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3copjndcq.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3miufdgry.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3euwdiqgr.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3xlqcgutd.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3bnlnpxpx.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3sxglsxft.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3jogeznwr.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3lnbjgsoz.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3sodtscrx.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3ycrngmhr.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3bgpsvoyb.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3ynmmiwsb.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3tssbjenv.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3ebldjbqc.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3nuavstyd.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3xhvcuqam.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3xezcucmy.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3wwgkxcow.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3qprwgnpa.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3evdkbcqh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jzfuksaa.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3qmqwymet.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vgemrcmm.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3pewuxxfh.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3cfwdfsjh.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3cueycnje.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3sfifijcz.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3olrslqkh.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3jdqyghsl.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3eyakhjzq.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3fxzocouj.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3xubechcz.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3oqsjbkaa.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3qcsrvahk.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3rpdcoipe.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3hmyylxxh.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3mwagfcrt.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3cqobiuum.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3bucmyost.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3heacwfdc.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3goqodsvr.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3xuzpfbyo.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3tsvhnday.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3nnwjwjli.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3fhmvfltg.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3nfzeawyf.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3arveiwtg.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3pdztqyuq.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3fgfvdtvh.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3mgsgyoay.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3wvsstqmh.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3vispsbul.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3euoawmjr.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3mzumykgq.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3peeuwoor.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3mktmtygf.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3anhmdbny.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jtoxvgoj.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ictimwcy.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3rnwsaofs.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3jwxuxuex.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3owenjevw.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3zsyzbjss.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3dlnvgkmf.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3psgdouhz.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3jbotkkkm.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3kjasjoxl.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3ayvwjogd.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3tipvzkmc.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3zqstwdxv.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3hfdniwtw.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3uvayrehf.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3vgilgozi.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3yexjviia.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3wiugrhyp.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3wcbxawbv.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3zxzfpvir.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3npcmazph.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3szwjwjoo.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ldbbagko.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3bumifxbk.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3yhwmpmsa.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3jarwfpnq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3cvsfpcyi.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3ykajzbef.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3zjtsxnsk.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3emfkremc.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3upbgaomy.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kwqiehdl.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3hfuschrb.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3abqvgqvg.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fkbfltrt.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3oiutpths.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3kmtohhpe.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3hqzsbthi.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3oquylixe.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3dfvebwfv.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3qzvncjkr.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3mddapmyp.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3lgcdyysb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xruyffrj.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3roqnyxrg.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3jjpfwvbf.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3plhgntsy.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3avcguywf.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3samhomeg.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3pwhxhnzz.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3bzjvjgnj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3pzivwoea.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3lhazaith.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3rfloggsy.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3yxfbujvz.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3spsgyukr.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3cmdeytui.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3cvruvmnz.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3mvtrhrlm.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3vnjnejul.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3guvjamgw.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3eixqezow.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3vhpmkycf.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3jtvuvhiy.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3cpucglel.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3mtpsnkso.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3hjenzwjj.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3gvftsdxl.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3amhibcex.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3hsnkxtoo.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3etletcfr.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3uvecbvsy.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3yuxuaibz.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3dgzgluro.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3gpbcurue.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3bmgrqfwt.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3uiexrqox.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3dhjakppd.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3nhnpphmt.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3hiukzpsd.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3dykrkxnj.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3lpusrxov.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3inydkzsm.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3mhcsfpwl.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3tzrvvpyn.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3wsblpflp.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3sciwnliq.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3ufdbziwu.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3wkypdaao.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3udlapvfh.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3ujgpwvrd.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3cjejemdw.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3uaddkixz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zfduifkv.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3cyffqjty.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bwfrplzw.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vfwleejk.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3bsxcmywh.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3htowbeon.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3obtgjsqa.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3dyrsqzao.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3syuaofac.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3euevwfej.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3qejcyslu.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3hhysmkzb.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3ojqpltmg.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3rcwdnksa.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3mslxwlpk.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3wjwfvhyy.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3kdbisgom.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3gkxpnuep.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3qhclngyl.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3ydkkmqpx.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3asiugaen.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3qmzlfgqw.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3uftkjusp.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3bhhuyxpr.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3fekfbdis.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3zhwkperf.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3blmrsdej.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3trwbhxnx.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tzwwrkya.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3szxkrjag.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3ryjrtrgl.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3zfmgeuwv.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3ouwssngq.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ejftuljg.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3kccebxkv.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3jcpgafdt.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3nomgutfe.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3bdoziqof.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3lthwonin.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3vyjuooco.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3hrmykiux.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3rrfqciqo.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3ociygglq.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3meimekef.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3pyoahshq.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3puxxrvpy.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3yktovsrt.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3vztmjigs.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3okaxtwwn.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3iogejwed.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3vchtvawn.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3nnfvmwzt.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3rmcuiqrl.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3yyyuiavk.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3yovxptdc.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3qifqbrgh.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3eihnwivj.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3jnhcbcmd.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3rxgnprnu.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3wheymuta.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3vmlobesx.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3cjdvgepn.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3gbvkcsbt.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kkxldxqj.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3rshmnwzn.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3btxnvmco.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3xfuufhjh.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3lqebkflt.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3rffmctuj.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3meudkqtu.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3sujwudvl.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3rfbqcjuc.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3sxjvyzux.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3bxcubjch.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3elwqsaha.html


<!-- 参考信息 -->