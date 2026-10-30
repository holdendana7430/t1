代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.hesvh.cn/Article/details/gkjwexfnw.sHtML

[R36] 并发执行多个任务
来源：http://m.share.hesvh.cn/Article/details/ghrbpuxbi.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.zdbjq.cn/Article/details/guvqxavwc.sHtML

[R37] 把输出赋给变量
来源：http://baike.zdbjq.cn/Article/details/gbpseiojz.sHtML

files=$(ls -1)
来源：http://www.blog.zdbjq.cn/Article/details/gclrpnupc.sHtML

[R38] 管道串联
来源：http://www.share.hesvh.cn/Article/details/ghmrxgbtv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.zdbjq.cn/Article/details/ggynzglur.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.zdbjq.cn/Article/details/gkdibpqug.sHtML

cmd > out.log 2>&1
来源：http://read.share.fehbvm.com/Article/details/gkkqnjqfy.sHtML

[R40] 追加写日志
来源：http://m.share.hesvh.cn/Article/details/gezlvasfl.sHtML

echo "log" >> out.log
来源：http://www.blog.zdbjq.cn/Article/details/gunqclljn.sHtML

[R41] 丢弃输出
来源：http://blog.hesvh.cn/Article/details/gfjngdnjy.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/ghdtjfwin.sHtML

[R42] 输入重定向
来源：http://3g.fehbvm.com/Article/details/gzrcphbxm.sHtML

wc -l < a.txt
来源：http://read.share.zdbjq.cn/Article/details/gfhhqhejh.sHtML

[R43] 按名字查找文件
来源：http://baike.hesvh.cn/Article/details/gdaovzyrr.sHtML

find . -name "*.log" -type f
来源：http://www.share.zdbjq.cn/Article/details/gxtgsczbj.sHtML

[R44] 按修改时间查找
来源：http://3g.fehbvm.com/Article/details/gjycugrgz.sHtML

find . -mtime -7 -type f
来源：http://mobile.fehbvm.com/Article/details/gondrwevn.sHtML

[R45] 批量删除
来源：http://read.share.zdbjq.cn/Article/details/gpdjnfjmu.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.hesvh.cn/Article/details/gvxplopsb.sHtML

[R46] 递归替换文件内容
来源：http://read.share.zdbjq.cn/Article/details/gzqzdhuzt.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.zdbjq.cn/Article/details/ggxgtpjgb.sHtML

[R47] sed 单行替换
来源：http://m.share.hesvh.cn/Article/details/gnvawvwgs.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.zdbjq.cn/Article/details/ggtliwrfy.sHtML

[R48] awk 取指定列
来源：http://www.m.share.zdbjq.cn/Article/details/gfjbgmncp.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.hesvh.cn/Article/details/gmrtnqagc.sHtML

[R49] awk 带条件
来源：http://3g.hesvh.cn/Article/details/guekpjxsw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.zdbjq.cn/Article/details/gvufuutls.sHtML

[R50] awk 求和
来源：http://www.m.share.hesvh.cn/Article/details/gpzvfahlk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/ggmbksfju.sHtML

[R51] 排序去重取前几
来源：http://mobile.zdbjq.cn/Article/details/gzinovpaw.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.zdbjq.cn/Article/details/grsznttis.sHtML

[R52] 统计行数
来源：http://blog.fehbvm.com/Article/details/gaozpxjqe.sHtML

wc -l a.txt
来源：http://wap.hesvh.cn/Article/details/gsshuytxk.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.hesvh.cn/Article/details/glvaboigu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.hesvh.cn/Article/details/gpsuxfxtv.sHtML

[R54] 比较两个文件
来源：http://baike.hesvh.cn/Article/details/guiaicvud.sHtML

diff a.txt b.txt
来源：http://mobile.hesvh.cn/Article/details/ggowetpwl.sHtML

[R55] 压缩与解压
来源：http://blog.fehbvm.com/Article/details/gctrcjirw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fehbvm.com/Article/details/gnxmfdlzz.sHtML

[R56] 远程拷贝
来源：http://www.share.zdbjq.cn/Article/details/gnbwkowey.sHtML

scp file user@host:/path/
来源：http://www.m.share.zdbjq.cn/Article/details/gzdgzphdm.sHtML

[R57] 远程执行命令
来源：http://www.share.fehbvm.com/Article/details/gezpaogxk.sHtML

ssh user@host 'uptime'
来源：http://www.share.hesvh.cn/Article/details/ghrubtiic.sHtML

[R58] 下载文件
来源：http://3g.fehbvm.com/Article/details/gyqeglthf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fehbvm.com/Article/details/gkrnbjdcb.sHtML

[R59] 发 POST JSON
来源：http://3g.fehbvm.com/Article/details/gxhinocor.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.hesvh.cn/Article/details/gurmlatia.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/gzbomowax.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.zdbjq.cn/Article/details/geobovshy.sHtML

[R61] 磁盘占用
来源：http://blog.hesvh.cn/Article/details/gqtydhstk.sHtML

df -h;  du -sh *
来源：http://wap.fehbvm.com/Article/details/gmywqgdye.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fehbvm.com/Article/details/gxboqmaxk.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.hesvh.cn/Article/details/gczoydkdd.sHtML

[R63] 内存与进程
来源：http://mobile.zdbjq.cn/Article/details/gndqvrkfp.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.hesvh.cn/Article/details/galrwzrbw.sHtML

[R64] 结束进程
来源：http://mobile.hesvh.cn/Article/details/gctvlqknp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.zdbjq.cn/Article/details/gcfyutxec.sHtML

[R65] 查看端口占用
来源：http://read.share.fehbvm.com/Article/details/gynjddpzg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fehbvm.com/Article/details/gduuxgdcr.sHtML

[R66] 定时任务
来源：http://blog.fehbvm.com/Article/details/grxpmlaqq.sHtML

crontab -e;  crontab -l
来源：http://3g.fehbvm.com/Article/details/gntbhsyem.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fehbvm.com/Article/details/gprdeqwdn.sHtML

openssl rand -hex 16
来源：http://wap.zdbjq.cn/Article/details/gqhwfyriv.sHtML

[R68] 计算文件校验值
来源：http://blog.fehbvm.com/Article/details/ghddguxue.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fehbvm.com/Article/details/grrdnsgqp.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fehbvm.com/Article/details/gyllvongp.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fehbvm.com/Article/details/gaklggkpe.sHtML

[R70] 时间戳与互转
来源：http://baike.hesvh.cn/Article/details/gippgzjxs.sHtML

date +%s;  date -d @1700000000
来源：http://baike.zdbjq.cn/Article/details/gjvapiezy.sHtML

[R71] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/gkqcezzkr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.zdbjq.cn/Article/details/gftnocwcc.sHtML

[R72] 等待端口就绪
来源：http://read.share.hesvh.cn/Article/details/gdnjcuofz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gzowvlddk.sHtML

[R73] 分割大日志
来源：http://baike.fehbvm.com/Article/details/glzoszfyg.sHtML

split -l 1000 big.log part_
来源：http://www.share.fehbvm.com/Article/details/gfaoqzdjj.sHtML

[R74] 批量重命名
来源：http://baike.zdbjq.cn/Article/details/ghhfyvxgi.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fehbvm.com/Article/details/gtfjczvpm.sHtML

[R75] 导出环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gqgehzbbi.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.zdbjq.cn/Article/details/ghdqjctir.sHtML

[R76] 使用临时文件
来源：http://www.share.hesvh.cn/Article/details/gmgjroiwh.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/geahitojk.sHtML

[R77] 读取用户输入
来源：http://www.m.share.hesvh.cn/Article/details/gexhmefga.sHtML

read -rp "请输入: " ans
来源：http://baike.hesvh.cn/Article/details/gjdhhjbxb.sHtML

[R78] 交互式菜单
来源：http://blog.hesvh.cn/Article/details/ghdyildws.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.hesvh.cn/Article/details/giumhptzx.sHtML

[R79] 解析命令行选项
来源：http://read.share.zdbjq.cn/Article/details/gmzvuuvsj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fehbvm.com/Article/details/gujbfkkrp.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.zdbjq.cn/Article/details/gtuvpzaxa.sHtML

time ./run.sh
来源：http://blog.zdbjq.cn/Article/details/gugfxosme.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gcttnlesx.sHtML

S. C / C++ 专题
来源：http://www.blog.zdbjq.cn/Article/details/grblmdgde.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gfdaaekiw.sHtML

[S01] C：Hello World
来源：http://www.blog.hesvh.cn/Article/details/grwmidmqd.sHtML

#include <stdio.h>
来源：http://baike.hesvh.cn/Article/details/gzcaftlrk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.zdbjq.cn/Article/details/gqvufhuve.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fehbvm.com/Article/details/gxkxawziu.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fehbvm.com/Article/details/gnansqbzg.sHtML

[S03] C：读入整数
来源：http://read.share.hesvh.cn/Article/details/gsrwajiya.sHtML

int x; scanf("%d", &x);
来源：http://blog.fehbvm.com/Article/details/gnarqsgnc.sHtML

[S04] C：字符串复制
来源：http://mobile.hesvh.cn/Article/details/gaiepbmzi.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.zdbjq.cn/Article/details/gkrrkyszt.sHtML

[S05] C：字符串长度
来源：http://wap.fehbvm.com/Article/details/gsdthhrbs.sHtML

strlen(s)
来源：http://baike.zdbjq.cn/Article/details/gyfrjlxqd.sHtML

[S06] C：字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gxfqfjmrq.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fehbvm.com/Article/details/gtejitgwb.sHtML

[S07] C：数组遍历求和
来源：http://baike.hesvh.cn/Article/details/goftuzszl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.hesvh.cn/Article/details/ggjflztrk.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.hesvh.cn/Article/details/gsaoesmpu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.zdbjq.cn/Article/details/gbgcsyofr.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.zdbjq.cn/Article/details/ghvvydudw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.zdbjq.cn/Article/details/ghqzonxqn.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.hesvh.cn/Article/details/gbxohbmci.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fehbvm.com/Article/details/gpprngiqv.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gxftlvwhd.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.zdbjq.cn/Article/details/guarpeugg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.zdbjq.cn/Article/details/gsnkbhlmf.sHtML

fclose(f);
来源：http://wap.zdbjq.cn/Article/details/gekkhzpor.sHtML

[S12] C：写文件
来源：http://3g.hesvh.cn/Article/details/gcmumaevr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.hesvh.cn/Article/details/goarwlexm.sHtML

[S13] C：宏定义
来源：http://m.share.hesvh.cn/Article/details/gytojhbas.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.zdbjq.cn/Article/details/gqavxnkzp.sHtML

[S14] C：枚举
来源：http://www.blog.hesvh.cn/Article/details/gzdanczsq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.hesvh.cn/Article/details/gayoutnqz.sHtML

[S15] C：类型转换
来源：http://read.share.hesvh.cn/Article/details/ggpudxwxz.sHtML

(double) a / b
来源：http://www.m.share.hesvh.cn/Article/details/genyxhiqz.sHtML

[S16] C：位操作置位
来源：http://baike.hesvh.cn/Article/details/gyfenafqu.sHtML

x |= (1 << 3);
来源：http://www.share.fehbvm.com/Article/details/gnmugmifw.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gbnpzkffv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.hesvh.cn/Article/details/gbcqasdvn.sHtML

[S18] C：命令行参数
来源：http://www.share.hesvh.cn/Article/details/gfbhxspyw.sHtML

int main(int argc, char **argv)
来源：http://3g.fehbvm.com/Article/details/gchuiefkk.sHtML

[S19] C：快速排序
来源：http://mobile.fehbvm.com/Article/details/gjtyciaiq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/gruyvwcgj.sHtML

[S20] C：二分查找
来源：http://read.share.hesvh.cn/Article/details/grqgnpznl.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/gzcuktyjt.sHtML

[S21] C：字符类别判断
来源：http://read.share.hesvh.cn/Article/details/glbcfkhea.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.hesvh.cn/Article/details/gurhmjznu.sHtML

[S22] C：字符串转数字
来源：http://www.share.zdbjq.cn/Article/details/gfvctqjsq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.zdbjq.cn/Article/details/guthzpkvy.sHtML

[S23] C：随机数
来源：http://www.blog.zdbjq.cn/Article/details/gmfjqaizf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.zdbjq.cn/Article/details/gjifovnxd.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.hesvh.cn/Article/details/gpzkqnzwg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.hesvh.cn/Article/details/gjifiwrel.sHtML

[S25] C：内存拷贝
来源：http://read.share.hesvh.cn/Article/details/gtgrpunpp.sHtML

memcpy(dst, src, n);
来源：http://blog.hesvh.cn/Article/details/gkmlulbnn.sHtML

[S26] C：内存清零
来源：http://www.share.hesvh.cn/Article/details/gctpfqdpx.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fehbvm.com/Article/details/ghtcaskee.sHtML

[S27] C：定义常量
来源：http://www.blog.fehbvm.com/Article/details/gtvqqiqss.sHtML

const double PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gtizgcbff.sHtML

[S28] C：静态变量
来源：http://3g.zdbjq.cn/Article/details/gzxyxsvgn.sHtML

static int counter = 0;
来源：http://www.m.share.fehbvm.com/Article/details/gibuqvpym.sHtML

[S29] C：变参函数
来源：http://baike.hesvh.cn/Article/details/gbxboxceb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.zdbjq.cn/Article/details/gpaqcwvtl.sHtML

[S30] C：头文件保护
来源：http://3g.hesvh.cn/Article/details/gxqgqrdcm.sHtML

#ifndef X_H
来源：http://www.blog.fehbvm.com/Article/details/gpzlbhpij.sHtML

#define X_H
来源：http://www.blog.fehbvm.com/Article/details/gihjjhrkx.sHtML

#endif
来源：http://blog.hesvh.cn/Article/details/gccimbmfq.sHtML

[S31] C++：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gfuorilhk.sHtML

#include <iostream>
来源：http://m.share.hesvh.cn/Article/details/gcszwevis.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.hesvh.cn/Article/details/gnhaiejka.sHtML

[S32] C++：字符串
来源：http://www.share.hesvh.cn/Article/details/ghxqdavnd.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fehbvm.com/Article/details/gwxgaxmsd.sHtML

[S33] C++：vector 增删
来源：http://mobile.zdbjq.cn/Article/details/gsfzimkth.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.hesvh.cn/Article/details/ggdokgclm.sHtML

[S34] C++：遍历 vector
来源：http://read.share.zdbjq.cn/Article/details/gcrzzopgk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.hesvh.cn/Article/details/gyfjponsd.sHtML

[S35] C++：map
来源：http://read.share.zdbjq.cn/Article/details/gtkzmqlch.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fehbvm.com/Article/details/ggstuuvcx.sHtML

[S36] C++：unordered_map
来源：http://blog.zdbjq.cn/Article/details/ghdjockis.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gxxgkwuys.sHtML

[S37] C++：set
来源：http://blog.zdbjq.cn/Article/details/gzhnttnxb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.hesvh.cn/Article/details/ghjktewen.sHtML

[S38] C++：排序
来源：http://blog.zdbjq.cn/Article/details/ginaklypu.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gztpkzily.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.hesvh.cn/Article/details/gjwpbquol.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.hesvh.cn/Article/details/grwerkebf.sHtML

[S40] C++：查找元素
来源：http://www.blog.hesvh.cn/Article/details/gfhbwrfdu.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fehbvm.com/Article/details/gykjpzqjm.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fehbvm.com/Article/details/gpygysjlm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.zdbjq.cn/Article/details/gowmgxbhq.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.zdbjq.cn/Article/details/ghfdwvvcg.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.zdbjq.cn/Article/details/guzljvtxr.sHtML

[S43] C++：智能指针
来源：http://www.m.share.zdbjq.cn/Article/details/gpkdzeumt.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.zdbjq.cn/Article/details/gsfipfmot.sHtML

[S44] C++：引用传参
来源：http://read.share.zdbjq.cn/Article/details/giwoymjgb.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fehbvm.com/Article/details/ggcmwmsqd.sHtML

[S45] C++：lambda
来源：http://read.share.fehbvm.com/Article/details/gfitfqwgb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.zdbjq.cn/Article/details/gesjhxzeo.sHtML

[S46] C++：函数模板
来源：http://wap.zdbjq.cn/Article/details/gowkkfege.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.zdbjq.cn/Article/details/gkiietfzy.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fehbvm.com/Article/details/geneooqqi.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.zdbjq.cn/Article/details/gnvcffslg.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gvkuwyfob.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.hesvh.cn/Article/details/gjeearrvq.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fehbvm.com/Article/details/grmpcuxrj.sHtML

[S49] C++：写文件
来源：http://wap.fehbvm.com/Article/details/gmfspezyc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fehbvm.com/Article/details/gwfxtwhtw.sHtML

[S50] C++：格式化数字
来源：http://3g.zdbjq.cn/Article/details/gvzfqczwt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.hesvh.cn/Article/details/gbotwtuaa.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fehbvm.com/Article/details/ghjmyrigc.sHtML

static_cast<double>(a) / b
来源：http://www.share.hesvh.cn/Article/details/gbvujvgad.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.hesvh.cn/Article/details/grmgqxxxz.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.hesvh.cn/Article/details/gkmswjacd.sHtML

[S53] C++：移动语义
来源：http://3g.hesvh.cn/Article/details/ganrdoney.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fehbvm.com/Article/details/guzcqdksv.sHtML

[S54] C++：异常处理
来源：http://3g.zdbjq.cn/Article/details/gtwlewmsm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.hesvh.cn/Article/details/ghfrjchar.sHtML

[S55] C++：结构化绑定
来源：http://m.share.hesvh.cn/Article/details/ghbxvkeyd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fehbvm.com/Article/details/ggezcpcmh.sHtML

[S56] C++：optional
来源：http://baike.fehbvm.com/Article/details/gmhqpopir.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.zdbjq.cn/Article/details/gafqzlylj.sHtML

[S57] C++：编译期常量
来源：http://www.blog.zdbjq.cn/Article/details/gfihpnciw.sHtML

constexpr int N = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/guzodistx.sHtML

[S58] C++：命名空间
来源：http://www.blog.fehbvm.com/Article/details/gwmfonomr.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fehbvm.com/Article/details/guljqhcyg.sHtML

[S59] C++：静态断言
来源：http://www.share.hesvh.cn/Article/details/gybtkerfo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.hesvh.cn/Article/details/gvwnkkddn.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fehbvm.com/Article/details/gdknprnee.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.zdbjq.cn/Article/details/gqtycrzhy.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gcqtecnts.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.zdbjq.cn/Article/details/gekgaemgl.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gbcrnzftr.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.hesvh.cn/Article/details/gissyfbqy.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gejdjswyf.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fehbvm.com/Article/details/gtsohmfgm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.hesvh.cn/Article/details/gjlekekvg.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fehbvm.com/Article/details/gfllubevj.sHtML

"值: $b"
来源：http://mobile.zdbjq.cn/Article/details/gyrrmrtha.sHtML

[T04] Kotlin：空安全
来源：http://3g.zdbjq.cn/Article/details/gigvbjzqi.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.hesvh.cn/Article/details/gzxrutgua.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fehbvm.com/Article/details/gpvedvkqv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.zdbjq.cn/Article/details/gflsvnjxd.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/gqiaicyzv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.zdbjq.cn/Article/details/gqehyeboq.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fehbvm.com/Article/details/gvowuwiko.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.zdbjq.cn/Article/details/gkxtfbaif.sHtML

[T08] Kotlin：数据类
来源：http://baike.zdbjq.cn/Article/details/gqgixsowr.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.hesvh.cn/Article/details/gpnxuehly.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.hesvh.cn/Article/details/gdqlwnkxa.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.zdbjq.cn/Article/details/gewyfldqt.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fehbvm.com/Article/details/glgmmsufm.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.hesvh.cn/Article/details/gevgjslmj.sHtML

[T11] Kotlin：协程
来源：http://wap.fehbvm.com/Article/details/guhvkwzct.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.zdbjq.cn/Article/details/gtozxvxzi.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.zdbjq.cn/Article/details/gmnswwvrn.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gicxckuyd.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.zdbjq.cn/Article/details/gwinbuenk.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.zdbjq.cn/Article/details/gxfgtvnge.sHtML

[T14] Kotlin：循环
来源：http://3g.hesvh.cn/Article/details/gufnfbink.sHtML

for (i in 1..10) println(i)
来源：http://wap.fehbvm.com/Article/details/gygcawzcd.sHtML

[T15] Kotlin：接口
来源：http://wap.zdbjq.cn/Article/details/gnfwrkabq.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fehbvm.com/Article/details/gobalfmpk.sHtML

[T16] Swift：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gqqrnkwtg.sHtML

print("Hello")
来源：http://blog.zdbjq.cn/Article/details/grjtudfsu.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fehbvm.com/Article/details/gzxfoszdm.sHtML

var a = 1;  let b = 2
来源：http://read.share.zdbjq.cn/Article/details/grgtjafga.sHtML

[T18] Swift：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gwlsxybxn.sHtML

"值: \(b)"
来源：http://www.blog.fehbvm.com/Article/details/grfrnyzze.sHtML

[T19] Swift：可选绑定
来源：http://3g.zdbjq.cn/Article/details/gooubpnat.sHtML

if let n = opt { print(n) }
来源：http://m.share.zdbjq.cn/Article/details/gkhldvmyj.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.zdbjq.cn/Article/details/ganohhwna.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.fehbvm.com/Article/details/grmkuepib.sHtML

[T21] Swift：遍历
来源：http://baike.fehbvm.com/Article/details/gnequozwc.sHtML

for x in a { print(x) }
来源：http://baike.fehbvm.com/Article/details/gqsnwgctq.sHtML

[T22] Swift：字典
来源：http://blog.fehbvm.com/Article/details/glcdlopad.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fehbvm.com/Article/details/gdaizfang.sHtML

[T23] Swift：函数
来源：http://m.share.zdbjq.cn/Article/details/gewfixxqq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gysgpjmsh.sHtML

[T24] Swift：闭包
来源：http://www.share.fehbvm.com/Article/details/gvntwaplg.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gyugyspab.sHtML

[T25] Swift：结构体
来源：http://blog.fehbvm.com/Article/details/gudaqrorx.sHtML

struct P { var x: Int }
来源：http://www.share.hesvh.cn/Article/details/gabctafiq.sHtML

[T26] Swift：类与重写
来源：http://www.share.zdbjq.cn/Article/details/gsnlgupbq.sHtML

class A: Base { override func f() {} }
来源：http://baike.fehbvm.com/Article/details/gllbkvcob.sHtML

[T27] Swift：错误处理
来源：http://blog.zdbjq.cn/Article/details/gfcxumcux.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.zdbjq.cn/Article/details/gpkjzatcd.sHtML

[T28] Swift：枚举
来源：http://m.share.fehbvm.com/Article/details/gbkwdvbqw.sHtML

enum Color { case red, green }
来源：http://mobile.fehbvm.com/Article/details/ginviryqv.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.hesvh.cn/Article/details/glfkbntyt.sHtML

guard let x = opt else { return }
来源：http://wap.zdbjq.cn/Article/details/gkcauwcnj.sHtML

[T30] Swift：协议
来源：http://www.m.share.zdbjq.cn/Article/details/gtdkzypdu.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fehbvm.com/Article/details/govmntptv.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gchxeioib.sHtML

print("Hello")
来源：http://read.share.fehbvm.com/Article/details/geeixdynj.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fehbvm.com/Article/details/gognvcvhv.sHtML

local a = 1
来源：http://m.share.hesvh.cn/Article/details/glmxanrqw.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.zdbjq.cn/Article/details/gssfrgqdf.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.hesvh.cn/Article/details/gxcgucjhq.sHtML

[T34] Lua：遍历表
来源：http://www.blog.zdbjq.cn/Article/details/gimldnpld.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.fehbvm.com/Article/details/gfibcgvkf.sHtML

[T35] Lua：字典表
来源：http://www.share.fehbvm.com/Article/details/ghucbcprs.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fehbvm.com/Article/details/gblibeysz.sHtML

[T36] Lua：函数
来源：http://3g.hesvh.cn/Article/details/guslqebrh.sHtML

function add(a, b) return a + b end
来源：http://www.blog.fehbvm.com/Article/details/gaonlyhnq.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.fehbvm.com/Article/details/grcrafcoy.sHtML

"a" .. "b"
来源：http://wap.hesvh.cn/Article/details/guxogsyqg.sHtML

[T38] Lua：条件
来源：http://3g.hesvh.cn/Article/details/gqtdennrq.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.fehbvm.com/Article/details/gowudcjep.sHtML


<!-- 参考信息 -->