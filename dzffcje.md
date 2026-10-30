代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fanxiaobao.xyz/Article/details/gccpzxotb.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gtwccrbqg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/gqniivdiz.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fanxiaobao.xyz/Article/details/guwwqiqne.sHtML

files=$(ls -1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gblxxivqv.sHtML

[R38] 管道串联
来源：http://baike.fanxiaobao.xyz/Article/details/gqvcrzphd.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxdmxxfat.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fanxiaobao.xyz/Article/details/gomtexbat.sHtML

cmd > out.log 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gpnhsnfdl.sHtML

[R40] 追加写日志
来源：http://3g.fanxiaobao.xyz/Article/details/giqnvkogk.sHtML

echo "log" >> out.log
来源：http://baike.fanxiaobao.xyz/Article/details/gbliowzjq.sHtML

[R41] 丢弃输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcqrcgpmc.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gucgtcneh.sHtML

[R42] 输入重定向
来源：http://baike.fanxiaobao.xyz/Article/details/gpgqmyjma.sHtML

wc -l < a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gyxusxqgy.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcmhrttms.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grwgdtcek.sHtML

[R44] 按修改时间查找
来源：http://read.share.fanxiaobao.xyz/Article/details/ggqqlsblp.sHtML

find . -mtime -7 -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/glfutvbpt.sHtML

[R45] 批量删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glwgxqjht.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fanxiaobao.xyz/Article/details/gcczkpcmn.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/gqvncejkd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fanxiaobao.xyz/Article/details/gnaxynyvx.sHtML

[R47] sed 单行替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gxrjsdtgy.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/grkzzuecr.sHtML

[R48] awk 取指定列
来源：http://blog.fanxiaobao.xyz/Article/details/gdttrfvpl.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqctdlpji.sHtML

[R49] awk 带条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojrwuhbo.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fanxiaobao.xyz/Article/details/ghawuzajs.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gedjnxdet.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gutlofqya.sHtML

[R51] 排序去重取前几
来源：http://blog.fanxiaobao.xyz/Article/details/gxcnqsngn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fanxiaobao.xyz/Article/details/ggjbpmsfm.sHtML

[R52] 统计行数
来源：http://3g.fanxiaobao.xyz/Article/details/gczersegg.sHtML

wc -l a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gewsijcuv.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gafppsgez.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fanxiaobao.xyz/Article/details/ggmzwvidt.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gqbemqtkv.sHtML

diff a.txt b.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gfwemgqjq.sHtML

[R55] 压缩与解压
来源：http://blog.fanxiaobao.xyz/Article/details/gxhxwihpa.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fanxiaobao.xyz/Article/details/gywjgdsfs.sHtML

[R56] 远程拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gdkssopgh.sHtML

scp file user@host:/path/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwkozxbix.sHtML

[R57] 远程执行命令
来源：http://www.blog.fanxiaobao.xyz/Article/details/glkdxrqaf.sHtML

ssh user@host 'uptime'
来源：http://mobile.fanxiaobao.xyz/Article/details/gqgbwctww.sHtML

[R58] 下载文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gihthgxmw.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqgnlkbg.sHtML

[R59] 发 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gqksfzucq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmcqixnzx.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmmojqsm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fanxiaobao.xyz/Article/details/gtldxllgl.sHtML

[R61] 磁盘占用
来源：http://blog.fanxiaobao.xyz/Article/details/gjcbwjnmi.sHtML

df -h;  du -sh *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/getzkudyu.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfizzizre.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fanxiaobao.xyz/Article/details/gdtgacnuv.sHtML

[R63] 内存与进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grosncxlo.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvtlwryxt.sHtML

[R64] 结束进程
来源：http://3g.fanxiaobao.xyz/Article/details/ggphnylal.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fanxiaobao.xyz/Article/details/gomnfbvbj.sHtML

[R65] 查看端口占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gcpqokmbq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fanxiaobao.xyz/Article/details/gjpewnxsu.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/grhyzovre.sHtML

crontab -e;  crontab -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gvcssdutw.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fanxiaobao.xyz/Article/details/gkidoygsw.sHtML

openssl rand -hex 16
来源：http://wap.fanxiaobao.xyz/Article/details/gyzkahytc.sHtML

[R68] 计算文件校验值
来源：http://baike.fanxiaobao.xyz/Article/details/ghxxuhzjc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gjjpwknca.sHtML

[R69] 生成随机密码
来源：http://baike.fanxiaobao.xyz/Article/details/gbgnitnpf.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fanxiaobao.xyz/Article/details/gdcboglst.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/gybevimcp.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fanxiaobao.xyz/Article/details/geckfoaku.sHtML

[R71] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gjutfzrzs.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fanxiaobao.xyz/Article/details/ghwjodmit.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/gqqrjzsoi.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gnlcyhvsu.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gosdgtlnp.sHtML

split -l 1000 big.log part_
来源：http://read.share.fanxiaobao.xyz/Article/details/gftjyyvct.sHtML

[R74] 批量重命名
来源：http://m.share.fanxiaobao.xyz/Article/details/gsiibejta.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gdipntwmu.sHtML

[R75] 导出环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gbhkglpvk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fanxiaobao.xyz/Article/details/grulkjgqw.sHtML

[R76] 使用临时文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gcoyrzzwp.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gcniuqkoh.sHtML

[R77] 读取用户输入
来源：http://blog.fanxiaobao.xyz/Article/details/gwgcegspu.sHtML

read -rp "请输入: " ans
来源：http://3g.fanxiaobao.xyz/Article/details/gcuflvlxl.sHtML

[R78] 交互式菜单
来源：http://mobile.fanxiaobao.xyz/Article/details/gqwtzkguc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gjzyelhcp.sHtML

[R79] 解析命令行选项
来源：http://wap.fanxiaobao.xyz/Article/details/gentclimf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fanxiaobao.xyz/Article/details/gtdrrooxv.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fanxiaobao.xyz/Article/details/gyjtcvqcr.sHtML

time ./run.sh
来源：http://3g.fanxiaobao.xyz/Article/details/gckcocodo.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gorqnbrgi.sHtML

S. C / C++ 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glehjobed.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gkyhpagda.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gupovjksx.sHtML

#include <stdio.h>
来源：http://blog.fanxiaobao.xyz/Article/details/gslnfjxzd.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fanxiaobao.xyz/Article/details/gdtktmwub.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gsixhjgbe.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fanxiaobao.xyz/Article/details/gyvjgnbgw.sHtML

[S03] C：读入整数
来源：http://3g.fanxiaobao.xyz/Article/details/gzlzdwtti.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gugqrywxy.sHtML

[S04] C：字符串复制
来源：http://mobile.fanxiaobao.xyz/Article/details/gibevurwy.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fanxiaobao.xyz/Article/details/gvmdmdlio.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gobqqiqty.sHtML

strlen(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glqmqvqrn.sHtML

[S06] C：字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzrfdqeus.sHtML

strcmp(a, b) == 0
来源：http://blog.fanxiaobao.xyz/Article/details/gsyiawdne.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwhvwned.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fanxiaobao.xyz/Article/details/gvhropirb.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fanxiaobao.xyz/Article/details/gdouhkbmp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnbtvrxn.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fanxiaobao.xyz/Article/details/gmfvfclht.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fanxiaobao.xyz/Article/details/gbxycdwoa.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkyupzdvq.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fanxiaobao.xyz/Article/details/gqqiukhtc.sHtML

[S11] C：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdplzpqj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fanxiaobao.xyz/Article/details/gosatqlrg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gnxnnznuw.sHtML

fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gclkpibuv.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gfxhffopu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gdjrkgfck.sHtML

[S13] C：宏定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gehfvgrim.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvufptkgw.sHtML

[S14] C：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gquwsispc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fanxiaobao.xyz/Article/details/gvhkbgoso.sHtML

[S15] C：类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcdvibfzi.sHtML

(double) a / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gkzxxcgnv.sHtML

[S16] C：位操作置位
来源：http://3g.fanxiaobao.xyz/Article/details/gavnyshgx.sHtML

x |= (1 << 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gaeryzuce.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaklocaty.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvgmtjiit.sHtML

[S18] C：命令行参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/grqdocauu.sHtML

int main(int argc, char **argv)
来源：http://3g.fanxiaobao.xyz/Article/details/gbpvppfdk.sHtML

[S19] C：快速排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gldknppzb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gzlvmrahp.sHtML

[S20] C：二分查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gmjowyuke.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gydxxztqi.sHtML

[S21] C：字符类别判断
来源：http://blog.fanxiaobao.xyz/Article/details/gubdvbhol.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fanxiaobao.xyz/Article/details/gxgauxkcd.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gtrxaoxjt.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/gavoykjxz.sHtML

[S23] C：随机数
来源：http://m.share.fanxiaobao.xyz/Article/details/gavbqkopx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfpeyoetq.sHtML

[S24] C：获取本地时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gptcpfess.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fanxiaobao.xyz/Article/details/guczfhxvg.sHtML

[S25] C：内存拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/ggrhvgmch.sHtML

memcpy(dst, src, n);
来源：http://mobile.fanxiaobao.xyz/Article/details/govcdwgzc.sHtML

[S26] C：内存清零
来源：http://www.share.fanxiaobao.xyz/Article/details/gvmcrtzpg.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fanxiaobao.xyz/Article/details/gwybfuckf.sHtML

[S27] C：定义常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gjgnedzrx.sHtML

const double PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gijvwdety.sHtML

[S28] C：静态变量
来源：http://3g.fanxiaobao.xyz/Article/details/gxttdkprv.sHtML

static int counter = 0;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfuwefqxb.sHtML

[S29] C：变参函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gajwhftov.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fanxiaobao.xyz/Article/details/gefrobhwu.sHtML

[S30] C：头文件保护
来源：http://m.share.fanxiaobao.xyz/Article/details/gmnenaldc.sHtML

#ifndef X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gyhdidvli.sHtML

#define X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gblihbano.sHtML

#endif
来源：http://wap.fanxiaobao.xyz/Article/details/gkzecwnpu.sHtML

[S31] C++：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gwicrkckr.sHtML

#include <iostream>
来源：http://baike.fanxiaobao.xyz/Article/details/garxxwyco.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fanxiaobao.xyz/Article/details/glnqkyqau.sHtML

[S32] C++：字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gjpdudgfm.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fanxiaobao.xyz/Article/details/gjbwualwk.sHtML

[S33] C++：vector 增删
来源：http://baike.fanxiaobao.xyz/Article/details/gpbccgobi.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gquqeerld.sHtML

[S34] C++：遍历 vector
来源：http://3g.fanxiaobao.xyz/Article/details/gvdfdjzap.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnhcjglno.sHtML

[S35] C++：map
来源：http://wap.fanxiaobao.xyz/Article/details/geqknvueb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gjugsjvlr.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqvjcylty.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghzldqhrm.sHtML

[S37] C++：set
来源：http://m.share.fanxiaobao.xyz/Article/details/gstpoqwhg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gkvkwjidl.sHtML

[S38] C++：排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gqdmnwtwk.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gaccsgbhk.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fanxiaobao.xyz/Article/details/gmzbosstp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwktldwy.sHtML

[S40] C++：查找元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gdgplsror.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwensdhom.sHtML

[S41] C++：类与构造函数
来源：http://3g.fanxiaobao.xyz/Article/details/gqqmddeoo.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gmugusfbe.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fanxiaobao.xyz/Article/details/giocfynai.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/gplnrvspq.sHtML

[S43] C++：智能指针
来源：http://mobile.fanxiaobao.xyz/Article/details/gsodimfyb.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fanxiaobao.xyz/Article/details/glselqctg.sHtML

[S44] C++：引用传参
来源：http://3g.fanxiaobao.xyz/Article/details/gzxbxhzpc.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzqtjlvhe.sHtML

[S45] C++：lambda
来源：http://3g.fanxiaobao.xyz/Article/details/gogtjxycd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbasrqzi.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gciromzow.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gchahticb.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcxtrqiir.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fanxiaobao.xyz/Article/details/gnkojnfkm.sHtML

[S48] C++：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gwanatlys.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fanxiaobao.xyz/Article/details/gepuotrne.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqitevyhh.sHtML

[S49] C++：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gjtinwpfs.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gxiaozovo.sHtML

[S50] C++：格式化数字
来源：http://wap.fanxiaobao.xyz/Article/details/gsyxujgrt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gqvazcaar.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gsbqsrhbt.sHtML

static_cast<double>(a) / b
来源：http://read.share.fanxiaobao.xyz/Article/details/ggpqcrnit.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fanxiaobao.xyz/Article/details/gvfoowwzf.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fanxiaobao.xyz/Article/details/giiyapvxp.sHtML

[S53] C++：移动语义
来源：http://baike.fanxiaobao.xyz/Article/details/gvdqkibin.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fanxiaobao.xyz/Article/details/ggzctbefc.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqpgnbflg.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fanxiaobao.xyz/Article/details/ggsljxwoo.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghpcgqmas.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gwdwsldyz.sHtML

[S56] C++：optional
来源：http://3g.fanxiaobao.xyz/Article/details/gddebhviw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gciuecbdh.sHtML

[S57] C++：编译期常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gvcavnavd.sHtML

constexpr int N = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/ghltwdxdh.sHtML

[S58] C++：命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/ggiipksni.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpunfewzo.sHtML

[S59] C++：静态断言
来源：http://3g.fanxiaobao.xyz/Article/details/gfjzowkau.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fanxiaobao.xyz/Article/details/gyhwuslqg.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fanxiaobao.xyz/Article/details/gysxxyouw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gvhiyyupc.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/ggtavnxwx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fanxiaobao.xyz/Article/details/gedjhxvde.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gzybmnoal.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnvnejhmo.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gqcqnwdgw.sHtML

[T02] Kotlin：变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gnnsaiehe.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fanxiaobao.xyz/Article/details/gqechtrrm.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gafyojvtv.sHtML

"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gzgawwswv.sHtML

[T04] Kotlin：空安全
来源：http://blog.fanxiaobao.xyz/Article/details/gnyfyutna.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fanxiaobao.xyz/Article/details/gdxodhrrk.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxvgvdhnl.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fanxiaobao.xyz/Article/details/gtuatxutg.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/gnuahbxvn.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gvyikwjok.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gktkkchfm.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxiyxllvo.sHtML

[T08] Kotlin：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/gyfazytuv.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/gslgfftnm.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fanxiaobao.xyz/Article/details/gaojhkufs.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fanxiaobao.xyz/Article/details/gsfcvbtnh.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fanxiaobao.xyz/Article/details/gtyhykikb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fanxiaobao.xyz/Article/details/gglkkiame.sHtML

[T11] Kotlin：协程
来源：http://read.share.fanxiaobao.xyz/Article/details/gdtefbxzt.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwkwzzryh.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fanxiaobao.xyz/Article/details/gfvdhluen.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggnhrjixs.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqpacnvj.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gjoyqevzb.sHtML

[T14] Kotlin：循环
来源：http://baike.fanxiaobao.xyz/Article/details/gwtpsihga.sHtML

for (i in 1..10) println(i)
来源：http://blog.fanxiaobao.xyz/Article/details/gnsxbdkyr.sHtML

[T15] Kotlin：接口
来源：http://baike.fanxiaobao.xyz/Article/details/grswwrcio.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fanxiaobao.xyz/Article/details/gemhwczrn.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkmehypqj.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gjmkqocho.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqjtcsdk.sHtML

var a = 1;  let b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gmnyinatt.sHtML

[T18] Swift：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gaxqstkoo.sHtML

"值: \(b)"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxfqtvuf.sHtML

[T19] Swift：可选绑定
来源：http://baike.fanxiaobao.xyz/Article/details/gttjiomah.sHtML

if let n = opt { print(n) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gaetuffne.sHtML

[T20] Swift：数组操作
来源：http://blog.fanxiaobao.xyz/Article/details/guabahhih.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guplpqqbo.sHtML

[T21] Swift：遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjhecvwrq.sHtML

for x in a { print(x) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbvnkvnih.sHtML

[T22] Swift：字典
来源：http://3g.fanxiaobao.xyz/Article/details/gfnuuzzbx.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gvtusklew.sHtML

[T23] Swift：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gzwmwzxir.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxpeahgge.sHtML

[T24] Swift：闭包
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcyjswher.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbtihtjmg.sHtML

[T25] Swift：结构体
来源：http://mobile.fanxiaobao.xyz/Article/details/gfhxbpcsl.sHtML

struct P { var x: Int }
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqfcetzc.sHtML

[T26] Swift：类与重写
来源：http://blog.fanxiaobao.xyz/Article/details/grgdyapnn.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghduynuws.sHtML

[T27] Swift：错误处理
来源：http://blog.fanxiaobao.xyz/Article/details/ggdywkixh.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggkoqsang.sHtML

[T28] Swift：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gwrolddzi.sHtML

enum Color { case red, green }
来源：http://wap.fanxiaobao.xyz/Article/details/gaszsijvv.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fanxiaobao.xyz/Article/details/gfpxvdhwr.sHtML

guard let x = opt else { return }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvfwxwgux.sHtML

[T30] Swift：协议
来源：http://3g.fanxiaobao.xyz/Article/details/gkfupamah.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/giypfsdeo.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvqdknwqt.sHtML

print("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwggrhmf.sHtML

[T32] Lua：局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gsglbexlc.sHtML

local a = 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywzxhlgp.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixthcygp.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fanxiaobao.xyz/Article/details/gfzxssdzx.sHtML

[T34] Lua：遍历表
来源：http://3g.fanxiaobao.xyz/Article/details/gzvxoybqv.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.fanxiaobao.xyz/Article/details/gcticahto.sHtML

[T35] Lua：字典表
来源：http://mobile.fanxiaobao.xyz/Article/details/gogxczube.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gpetqhmre.sHtML

[T36] Lua：函数
来源：http://blog.fanxiaobao.xyz/Article/details/ghezvpkdp.sHtML

function add(a, b) return a + b end
来源：http://m.share.fanxiaobao.xyz/Article/details/gevbopdkw.sHtML

[T37] Lua：字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/gjcwlykvt.sHtML

"a" .. "b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gjertpyco.sHtML

[T38] Lua：条件
来源：http://3g.fanxiaobao.xyz/Article/details/gvpelbbub.sHtML

if x > 0 then print("正") end
来源：http://3g.fanxiaobao.xyz/Article/details/gwssovxwr.sHtML


<!-- 参考信息 -->