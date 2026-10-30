代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.zdbjq.cn/Article/details/gmjtqazqs.sHtML

[R34] 退出时清理
来源：http://www.m.share.zdbjq.cn/Article/details/ggcejzckn.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/gayrmehhs.sHtML

[R35] 后台执行并等待
来源：http://read.share.zdbjq.cn/Article/details/gedlwqhlc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fehbvm.com/Article/details/gjzwebywy.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fehbvm.com/Article/details/gmlwecwaf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fehbvm.com/Article/details/gtgbzurqp.sHtML

[R37] 把输出赋给变量
来源：http://blog.hesvh.cn/Article/details/gwryiefdb.sHtML

files=$(ls -1)
来源：http://blog.hesvh.cn/Article/details/gdwssuayh.sHtML

[R38] 管道串联
来源：http://mobile.zdbjq.cn/Article/details/gsdtruetx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.hesvh.cn/Article/details/grzusbvvy.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.hesvh.cn/Article/details/gnvexucqg.sHtML

cmd > out.log 2>&1
来源：http://3g.fehbvm.com/Article/details/gffsjnkvv.sHtML

[R40] 追加写日志
来源：http://blog.fehbvm.com/Article/details/gsrkacqmx.sHtML

echo "log" >> out.log
来源：http://mobile.hesvh.cn/Article/details/gdmgfbrzk.sHtML

[R41] 丢弃输出
来源：http://m.share.zdbjq.cn/Article/details/guzunlwuh.sHtML

cmd >/dev/null 2>&1
来源：http://baike.hesvh.cn/Article/details/gdjnhxzif.sHtML

[R42] 输入重定向
来源：http://www.share.hesvh.cn/Article/details/gekkiboiq.sHtML

wc -l < a.txt
来源：http://www.share.fehbvm.com/Article/details/gwgdmrzlw.sHtML

[R43] 按名字查找文件
来源：http://www.share.fehbvm.com/Article/details/gnbijunss.sHtML

find . -name "*.log" -type f
来源：http://wap.fehbvm.com/Article/details/gifyfdvys.sHtML

[R44] 按修改时间查找
来源：http://m.share.hesvh.cn/Article/details/gdoprlvzo.sHtML

find . -mtime -7 -type f
来源：http://wap.fehbvm.com/Article/details/gfpsxiyav.sHtML

[R45] 批量删除
来源：http://www.share.zdbjq.cn/Article/details/gaqndokpa.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fehbvm.com/Article/details/gzmryjfuq.sHtML

[R46] 递归替换文件内容
来源：http://mobile.hesvh.cn/Article/details/guvfqyiyn.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.hesvh.cn/Article/details/gifoziuxu.sHtML

[R47] sed 单行替换
来源：http://mobile.hesvh.cn/Article/details/gyfyupiqm.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.hesvh.cn/Article/details/gwqbnokzh.sHtML

[R48] awk 取指定列
来源：http://m.share.zdbjq.cn/Article/details/guovrontv.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gmudcvgni.sHtML

[R49] awk 带条件
来源：http://baike.fehbvm.com/Article/details/gdlzfdhwc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.zdbjq.cn/Article/details/gwdmiycbd.sHtML

[R50] awk 求和
来源：http://www.blog.fehbvm.com/Article/details/gclelzyxe.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gvwfzlkfu.sHtML

[R51] 排序去重取前几
来源：http://3g.hesvh.cn/Article/details/gbvmthcck.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.hesvh.cn/Article/details/grjqehpel.sHtML

[R52] 统计行数
来源：http://wap.zdbjq.cn/Article/details/gyvpnklig.sHtML

wc -l a.txt
来源：http://baike.hesvh.cn/Article/details/gujgfkrvn.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.zdbjq.cn/Article/details/gcaaevyzv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.hesvh.cn/Article/details/gulbjorld.sHtML

[R54] 比较两个文件
来源：http://m.share.hesvh.cn/Article/details/gzbhayrbk.sHtML

diff a.txt b.txt
来源：http://3g.fehbvm.com/Article/details/gygqnevxx.sHtML

[R55] 压缩与解压
来源：http://3g.zdbjq.cn/Article/details/ggyjtxkjy.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fehbvm.com/Article/details/gkxwutewy.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gbzwznrbt.sHtML

scp file user@host:/path/
来源：http://www.share.hesvh.cn/Article/details/gqeeurlcy.sHtML

[R57] 远程执行命令
来源：http://mobile.hesvh.cn/Article/details/giiugqpjw.sHtML

ssh user@host 'uptime'
来源：http://m.share.fehbvm.com/Article/details/gjeoknhhj.sHtML

[R58] 下载文件
来源：http://mobile.fehbvm.com/Article/details/gtuahisqv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fehbvm.com/Article/details/gfsocfqdg.sHtML

[R59] 发 POST JSON
来源：http://wap.fehbvm.com/Article/details/gvxbixrww.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.hesvh.cn/Article/details/grxgocdyp.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gogmnomug.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fehbvm.com/Article/details/gxdklpazy.sHtML

[R61] 磁盘占用
来源：http://read.share.hesvh.cn/Article/details/gavivvhzb.sHtML

df -h;  du -sh *
来源：http://blog.fehbvm.com/Article/details/gyenhneiv.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fehbvm.com/Article/details/giaydlxzo.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.zdbjq.cn/Article/details/gdjnbiwve.sHtML

[R63] 内存与进程
来源：http://m.share.fehbvm.com/Article/details/gamcfnfca.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.hesvh.cn/Article/details/grtovntzu.sHtML

[R64] 结束进程
来源：http://m.share.hesvh.cn/Article/details/gztajeakp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.hesvh.cn/Article/details/grcommeju.sHtML

[R65] 查看端口占用
来源：http://baike.zdbjq.cn/Article/details/gawmqmptn.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fehbvm.com/Article/details/gnhhfkumi.sHtML

[R66] 定时任务
来源：http://mobile.zdbjq.cn/Article/details/gylvkfhnj.sHtML

crontab -e;  crontab -l
来源：http://blog.hesvh.cn/Article/details/gxncrtqab.sHtML

[R67] 生成随机十六进制串
来源：http://3g.hesvh.cn/Article/details/gxnzkyork.sHtML

openssl rand -hex 16
来源：http://blog.zdbjq.cn/Article/details/gkhpgrety.sHtML

[R68] 计算文件校验值
来源：http://blog.fehbvm.com/Article/details/gpzjfuzlr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.hesvh.cn/Article/details/gvwvcsnfa.sHtML

[R69] 生成随机密码
来源：http://www.share.fehbvm.com/Article/details/gljwbpxng.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.zdbjq.cn/Article/details/gnjxcxifz.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fehbvm.com/Article/details/gqgyntunv.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.zdbjq.cn/Article/details/gdebzwndm.sHtML

[R71] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gdwsmsmqo.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fehbvm.com/Article/details/gmmacfdil.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fehbvm.com/Article/details/gbtihvsfs.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/gmqzzsjpy.sHtML

[R73] 分割大日志
来源：http://www.blog.hesvh.cn/Article/details/gefjkojzt.sHtML

split -l 1000 big.log part_
来源：http://m.share.hesvh.cn/Article/details/gddfsrknk.sHtML

[R74] 批量重命名
来源：http://read.share.fehbvm.com/Article/details/gaifjnfgh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.zdbjq.cn/Article/details/goljinsmf.sHtML

[R75] 导出环境变量
来源：http://3g.fehbvm.com/Article/details/gfcxwmczl.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.hesvh.cn/Article/details/gfghlldur.sHtML

[R76] 使用临时文件
来源：http://read.share.hesvh.cn/Article/details/gxchnscfi.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/gbeakhwkj.sHtML

[R77] 读取用户输入
来源：http://blog.fehbvm.com/Article/details/goendbpoi.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.hesvh.cn/Article/details/gvuluwxqc.sHtML

[R78] 交互式菜单
来源：http://www.m.share.zdbjq.cn/Article/details/gacziyjzq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fehbvm.com/Article/details/gzesnkvwb.sHtML

[R79] 解析命令行选项
来源：http://www.share.hesvh.cn/Article/details/gqttssyup.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.hesvh.cn/Article/details/gpfxehgql.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fehbvm.com/Article/details/gfqfsanvr.sHtML

time ./run.sh
来源：http://wap.fehbvm.com/Article/details/gdpntvwxp.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gcjjymjan.sHtML

S. C / C++ 专题
来源：http://baike.zdbjq.cn/Article/details/gkqvkvgba.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gzaanyrzx.sHtML

[S01] C：Hello World
来源：http://m.share.fehbvm.com/Article/details/gzwbauefn.sHtML

#include <stdio.h>
来源：http://wap.hesvh.cn/Article/details/govvtydhq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.hesvh.cn/Article/details/gfjxfzigi.sHtML

[S02] C：变量与格式化输出
来源：http://baike.hesvh.cn/Article/details/ghhdbpwbi.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fehbvm.com/Article/details/gidoozyio.sHtML

[S03] C：读入整数
来源：http://www.share.fehbvm.com/Article/details/gjhuqxxzg.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fehbvm.com/Article/details/gvlrvhvek.sHtML

[S04] C：字符串复制
来源：http://www.blog.zdbjq.cn/Article/details/gcvfepjgt.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.zdbjq.cn/Article/details/gjepzxfaj.sHtML

[S05] C：字符串长度
来源：http://m.share.fehbvm.com/Article/details/grkzfndhn.sHtML

strlen(s)
来源：http://baike.zdbjq.cn/Article/details/gnuisglyw.sHtML

[S06] C：字符串比较
来源：http://read.share.fehbvm.com/Article/details/guentynzp.sHtML

strcmp(a, b) == 0
来源：http://mobile.hesvh.cn/Article/details/gqdxisgwi.sHtML

[S07] C：数组遍历求和
来源：http://read.share.hesvh.cn/Article/details/gkurlcayu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.zdbjq.cn/Article/details/gnlvluwwv.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.zdbjq.cn/Article/details/gxkwwzkfe.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.zdbjq.cn/Article/details/gdysjizus.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.hesvh.cn/Article/details/grlxxhxwe.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fehbvm.com/Article/details/ghmewfxrz.sHtML

[S10] C：指针与解引用
来源：http://blog.fehbvm.com/Article/details/gppgidgrq.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fehbvm.com/Article/details/gucmjtgmz.sHtML

[S11] C：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gtqatuvop.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.hesvh.cn/Article/details/grgtvtfwk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.zdbjq.cn/Article/details/ghfgsibex.sHtML

fclose(f);
来源：http://read.share.hesvh.cn/Article/details/gicunglfm.sHtML

[S12] C：写文件
来源：http://blog.zdbjq.cn/Article/details/gdpfziecc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/gzhjcaqxa.sHtML

[S13] C：宏定义
来源：http://www.blog.zdbjq.cn/Article/details/gxcrevlgn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fehbvm.com/Article/details/gazdyptdm.sHtML

[S14] C：枚举
来源：http://read.share.hesvh.cn/Article/details/givzueclb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.zdbjq.cn/Article/details/glnonqsnl.sHtML

[S15] C：类型转换
来源：http://baike.fehbvm.com/Article/details/gjiqzlnlq.sHtML

(double) a / b
来源：http://www.share.fehbvm.com/Article/details/gacmfxzvp.sHtML

[S16] C：位操作置位
来源：http://3g.hesvh.cn/Article/details/gimgcmgtf.sHtML

x |= (1 << 3);
来源：http://read.share.zdbjq.cn/Article/details/gygxwjwxt.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gjsiimfjp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fehbvm.com/Article/details/gudpzppaz.sHtML

[S18] C：命令行参数
来源：http://wap.hesvh.cn/Article/details/gzssvzhna.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fehbvm.com/Article/details/gaybgsnay.sHtML

[S19] C：快速排序
来源：http://wap.fehbvm.com/Article/details/glzuqefkx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gbqiiyoab.sHtML

[S20] C：二分查找
来源：http://3g.zdbjq.cn/Article/details/grnsrrnyp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gccbrkrar.sHtML

[S21] C：字符类别判断
来源：http://www.share.hesvh.cn/Article/details/glbmybdvv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.hesvh.cn/Article/details/ggmyergnb.sHtML

[S22] C：字符串转数字
来源：http://3g.fehbvm.com/Article/details/gtysudrft.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.hesvh.cn/Article/details/gprnbkvhs.sHtML

[S23] C：随机数
来源：http://baike.zdbjq.cn/Article/details/gopnvaorv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.zdbjq.cn/Article/details/gyfsvjosy.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.zdbjq.cn/Article/details/gymmudcsq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.hesvh.cn/Article/details/gqptepnpq.sHtML

[S25] C：内存拷贝
来源：http://mobile.zdbjq.cn/Article/details/gcctioaxs.sHtML

memcpy(dst, src, n);
来源：http://read.share.zdbjq.cn/Article/details/golayszbm.sHtML

[S26] C：内存清零
来源：http://blog.fehbvm.com/Article/details/gloinlfhh.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.zdbjq.cn/Article/details/gxzfdxnog.sHtML

[S27] C：定义常量
来源：http://baike.fehbvm.com/Article/details/gemcrtegx.sHtML

const double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gzcrsdptq.sHtML

[S28] C：静态变量
来源：http://www.m.share.zdbjq.cn/Article/details/gcmxagzui.sHtML

static int counter = 0;
来源：http://www.blog.zdbjq.cn/Article/details/gfkpjhkxu.sHtML

[S29] C：变参函数
来源：http://mobile.zdbjq.cn/Article/details/gpwdqnshr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fehbvm.com/Article/details/gbsapobam.sHtML

[S30] C：头文件保护
来源：http://3g.hesvh.cn/Article/details/gugapuavh.sHtML

#ifndef X_H
来源：http://blog.zdbjq.cn/Article/details/grtkzlmmn.sHtML

#define X_H
来源：http://m.share.fehbvm.com/Article/details/gyafhwuuf.sHtML

#endif
来源：http://baike.zdbjq.cn/Article/details/gvgdocvcz.sHtML

[S31] C++：Hello World
来源：http://baike.fehbvm.com/Article/details/gcqdtzufw.sHtML

#include <iostream>
来源：http://wap.fehbvm.com/Article/details/gbwkpcwfs.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.hesvh.cn/Article/details/gnqqxjahw.sHtML

[S32] C++：字符串
来源：http://mobile.fehbvm.com/Article/details/gcdbauckd.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.zdbjq.cn/Article/details/gbqnegkto.sHtML

[S33] C++：vector 增删
来源：http://read.share.zdbjq.cn/Article/details/gontjmojh.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.hesvh.cn/Article/details/ggoxsbylt.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fehbvm.com/Article/details/ggdjnaflw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.hesvh.cn/Article/details/gliccvgtg.sHtML

[S35] C++：map
来源：http://baike.fehbvm.com/Article/details/gvlwaxtno.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/ghygewivp.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fehbvm.com/Article/details/grxiwhofi.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/glsfdaauz.sHtML

[S37] C++：set
来源：http://www.share.hesvh.cn/Article/details/gahhhmezk.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fehbvm.com/Article/details/gwevsjmsp.sHtML

[S38] C++：排序
来源：http://baike.hesvh.cn/Article/details/gekrjadxb.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fehbvm.com/Article/details/ggdkbpnsm.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.hesvh.cn/Article/details/grmxjpaeo.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fehbvm.com/Article/details/gzyplmfhb.sHtML

[S40] C++：查找元素
来源：http://blog.fehbvm.com/Article/details/gnxxumqmv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.hesvh.cn/Article/details/gaaucyafw.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gfqytjpkc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fehbvm.com/Article/details/gprohfkff.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.hesvh.cn/Article/details/gbdccaybb.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fehbvm.com/Article/details/gusquxgph.sHtML

[S43] C++：智能指针
来源：http://blog.hesvh.cn/Article/details/ghfvzuzod.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.hesvh.cn/Article/details/gklydvuen.sHtML

[S44] C++：引用传参
来源：http://read.share.zdbjq.cn/Article/details/gaegelagp.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fehbvm.com/Article/details/glfontvnq.sHtML

[S45] C++：lambda
来源：http://www.m.share.hesvh.cn/Article/details/glxmskqlv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.hesvh.cn/Article/details/ggezjuvmw.sHtML

[S46] C++：函数模板
来源：http://www.m.share.hesvh.cn/Article/details/gbqzwfali.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.hesvh.cn/Article/details/geajcvkxr.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fehbvm.com/Article/details/grkzwdxxb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.hesvh.cn/Article/details/gwwvzxxjc.sHtML

[S48] C++：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gtjjucbtr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fehbvm.com/Article/details/gpwaeiton.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fehbvm.com/Article/details/gymzrldub.sHtML

[S49] C++：写文件
来源：http://wap.zdbjq.cn/Article/details/gwcgrivkl.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fehbvm.com/Article/details/gvgalblil.sHtML

[S50] C++：格式化数字
来源：http://baike.fehbvm.com/Article/details/gogfguzwy.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gywcurxtu.sHtML

[S51] C++：显式类型转换
来源：http://blog.fehbvm.com/Article/details/gcthkuejs.sHtML

static_cast<double>(a) / b
来源：http://www.share.fehbvm.com/Article/details/grsmebebn.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.zdbjq.cn/Article/details/gnrsulgfi.sHtML

int size() const noexcept { return n_; }
来源：http://3g.hesvh.cn/Article/details/gceafxeln.sHtML

[S53] C++：移动语义
来源：http://www.share.zdbjq.cn/Article/details/ggezfjcec.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.hesvh.cn/Article/details/gjgoeqgea.sHtML

[S54] C++：异常处理
来源：http://mobile.zdbjq.cn/Article/details/gjjemmtis.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.hesvh.cn/Article/details/gagfkahsh.sHtML

[S55] C++：结构化绑定
来源：http://3g.fehbvm.com/Article/details/gzfeeisto.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.zdbjq.cn/Article/details/gyylefdro.sHtML

[S56] C++：optional
来源：http://wap.zdbjq.cn/Article/details/gytgflxyx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.hesvh.cn/Article/details/gfmxyzgno.sHtML

[S57] C++：编译期常量
来源：http://www.share.fehbvm.com/Article/details/gatqufhbq.sHtML

constexpr int N = 10;
来源：http://www.share.hesvh.cn/Article/details/gsjdfbmgk.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fehbvm.com/Article/details/gsgjonmfv.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.zdbjq.cn/Article/details/gyjwgndla.sHtML

[S59] C++：静态断言
来源：http://blog.zdbjq.cn/Article/details/gaijlnmvy.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.hesvh.cn/Article/details/gchdmxqnq.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.zdbjq.cn/Article/details/gdhmzaaez.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.hesvh.cn/Article/details/grlleqxkz.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gjxxryacg.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fehbvm.com/Article/details/gcpnoegwa.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gobgbrrfz.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.hesvh.cn/Article/details/gnekuvbbh.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/gjtehylqb.sHtML

[T02] Kotlin：变量
来源：http://baike.hesvh.cn/Article/details/gubionqtq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.zdbjq.cn/Article/details/gkctrbale.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.hesvh.cn/Article/details/gplxkkmcx.sHtML

"值: $b"
来源：http://blog.hesvh.cn/Article/details/gnhvbtgdj.sHtML

[T04] Kotlin：空安全
来源：http://wap.zdbjq.cn/Article/details/gcpnevhkm.sHtML

val n: String? = null;  n?.length
来源：http://baike.zdbjq.cn/Article/details/gslctsfax.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gaqeuugia.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.hesvh.cn/Article/details/gyqkttozb.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fehbvm.com/Article/details/gbbppfuie.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.hesvh.cn/Article/details/gsjkwzznk.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fehbvm.com/Article/details/goctaflkx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/gqpgyygcn.sHtML

[T08] Kotlin：数据类
来源：http://baike.zdbjq.cn/Article/details/guyfqgpxt.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.zdbjq.cn/Article/details/gfeccwrah.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fehbvm.com/Article/details/grodizckr.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.hesvh.cn/Article/details/gazwwdloe.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.zdbjq.cn/Article/details/gxcsasmvb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fehbvm.com/Article/details/gohhhinsl.sHtML

[T11] Kotlin：协程
来源：http://blog.hesvh.cn/Article/details/ghqdbbzon.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.zdbjq.cn/Article/details/gbwftmdjs.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fehbvm.com/Article/details/gtyfifrwm.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gumbfciya.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.zdbjq.cn/Article/details/ghxitsmgq.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fehbvm.com/Article/details/gqkwhblja.sHtML

[T14] Kotlin：循环
来源：http://m.share.fehbvm.com/Article/details/gmsbtdvrd.sHtML

for (i in 1..10) println(i)
来源：http://read.share.zdbjq.cn/Article/details/gxedntdpd.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fehbvm.com/Article/details/geovvjevz.sHtML

interface Shape { fun area(): Double }
来源：http://baike.zdbjq.cn/Article/details/gjwtzrymj.sHtML

[T16] Swift：Hello World
来源：http://read.share.fehbvm.com/Article/details/gnjqfqnax.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gksdtrbwx.sHtML

[T17] Swift：变量与常量
来源：http://3g.hesvh.cn/Article/details/gfzvpmtwy.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fehbvm.com/Article/details/gnypuadwj.sHtML

[T18] Swift：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gubknhzxw.sHtML

"值: \(b)"
来源：http://baike.zdbjq.cn/Article/details/gcfsljhjg.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.hesvh.cn/Article/details/grmjlnfbx.sHtML

if let n = opt { print(n) }
来源：http://www.share.fehbvm.com/Article/details/ggmjifief.sHtML

[T20] Swift：数组操作
来源：http://baike.hesvh.cn/Article/details/grhebolqm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gihxmztox.sHtML

[T21] Swift：遍历
来源：http://www.share.zdbjq.cn/Article/details/gqiinbkic.sHtML

for x in a { print(x) }
来源：http://baike.zdbjq.cn/Article/details/gtoseroyw.sHtML

[T22] Swift：字典
来源：http://mobile.zdbjq.cn/Article/details/gtsdeujxw.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fehbvm.com/Article/details/gxeusyuip.sHtML

[T23] Swift：函数
来源：http://wap.hesvh.cn/Article/details/gnhugevhe.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fehbvm.com/Article/details/gyrlswnel.sHtML

[T24] Swift：闭包
来源：http://wap.zdbjq.cn/Article/details/gmjnltjnd.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/ghelyvikw.sHtML

[T25] Swift：结构体
来源：http://www.blog.zdbjq.cn/Article/details/grzyzatjm.sHtML

struct P { var x: Int }
来源：http://blog.fehbvm.com/Article/details/gbytqajex.sHtML

[T26] Swift：类与重写
来源：http://blog.fehbvm.com/Article/details/gshaesafd.sHtML

class A: Base { override func f() {} }
来源：http://www.share.hesvh.cn/Article/details/gyvdmfagj.sHtML

[T27] Swift：错误处理
来源：http://wap.fehbvm.com/Article/details/giszsivzb.sHtML

do { try f() } catch { print(error) }
来源：http://blog.hesvh.cn/Article/details/gojygpswz.sHtML

[T28] Swift：枚举
来源：http://baike.fehbvm.com/Article/details/gnnlnyixg.sHtML

enum Color { case red, green }
来源：http://www.m.share.hesvh.cn/Article/details/giynagtmp.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fehbvm.com/Article/details/ggcdawgsg.sHtML

guard let x = opt else { return }
来源：http://mobile.hesvh.cn/Article/details/gnefsxiba.sHtML

[T30] Swift：协议
来源：http://baike.hesvh.cn/Article/details/gwqlxxaim.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.fehbvm.com/Article/details/gaqetrqmb.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/grbskoaha.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gkmzokjpn.sHtML

[T32] Lua：局部变量
来源：http://3g.fehbvm.com/Article/details/gnanqickj.sHtML

local a = 1
来源：http://3g.hesvh.cn/Article/details/gjzkcgdpc.sHtML

[T33] Lua：表（数组）
来源：http://wap.fehbvm.com/Article/details/gstlwcpaq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.zdbjq.cn/Article/details/gaflhschc.sHtML

[T34] Lua：遍历表
来源：http://www.share.fehbvm.com/Article/details/gdrabxlww.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.hesvh.cn/Article/details/gbfbyuaoo.sHtML

[T35] Lua：字典表
来源：http://wap.hesvh.cn/Article/details/giqdctdrn.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.zdbjq.cn/Article/details/ggqjalmlm.sHtML

[T36] Lua：函数
来源：http://baike.fehbvm.com/Article/details/gkzmgbhjb.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.hesvh.cn/Article/details/gcvykojiy.sHtML


<!-- 参考信息 -->