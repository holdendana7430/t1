代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fanxiaobao.xyz/Article/details/goiamasxt.sHtML

[R34] 退出时清理
来源：http://mobile.fanxiaobao.xyz/Article/details/gofzpjbbx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/grzlpxved.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzrkfeyqv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fanxiaobao.xyz/Article/details/gibstwjyh.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fanxiaobao.xyz/Article/details/guloecgnt.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fanxiaobao.xyz/Article/details/gxkoppjra.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvjjocflj.sHtML

files=$(ls -1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxgjzwhzv.sHtML

[R38] 管道串联
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwaviobrw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fanxiaobao.xyz/Article/details/gctseuepw.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gvcfnrnaq.sHtML

cmd > out.log 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gehcbfgcp.sHtML

[R40] 追加写日志
来源：http://3g.fanxiaobao.xyz/Article/details/gdbcjpqlj.sHtML

echo "log" >> out.log
来源：http://wap.fanxiaobao.xyz/Article/details/gdlixqrtu.sHtML

[R41] 丢弃输出
来源：http://blog.fanxiaobao.xyz/Article/details/gvzerlnme.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gpbwfhuuw.sHtML

[R42] 输入重定向
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvhegacq.sHtML

wc -l < a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gqvqspmwl.sHtML

[R43] 按名字查找文件
来源：http://m.share.fanxiaobao.xyz/Article/details/glduqugcc.sHtML

find . -name "*.log" -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gzsrttrtz.sHtML

[R44] 按修改时间查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gsgsbxbmz.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/ghmfxmuqd.sHtML

[R45] 批量删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gxsmpbmas.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fanxiaobao.xyz/Article/details/gzduqijjl.sHtML

[R46] 递归替换文件内容
来源：http://wap.fanxiaobao.xyz/Article/details/gmavodise.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fanxiaobao.xyz/Article/details/gnmqqpylj.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtlcigjkn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gcrglipco.sHtML

[R48] awk 取指定列
来源：http://www.share.fanxiaobao.xyz/Article/details/gzboukneu.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gfgunqoip.sHtML

[R49] awk 带条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gglcznbzw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fanxiaobao.xyz/Article/details/gkaskvoau.sHtML

[R50] awk 求和
来源：http://wap.fanxiaobao.xyz/Article/details/gplgzwcli.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gagluyhrk.sHtML

[R51] 排序去重取前几
来源：http://wap.fanxiaobao.xyz/Article/details/gumbbaobv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqiomujqq.sHtML

[R52] 统计行数
来源：http://m.share.fanxiaobao.xyz/Article/details/gvbosanwb.sHtML

wc -l a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gvwpzxzjh.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fanxiaobao.xyz/Article/details/gbwgmmyzb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gkslmyhkj.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gickjuypr.sHtML

diff a.txt b.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gfgzfmonc.sHtML

[R55] 压缩与解压
来源：http://wap.fanxiaobao.xyz/Article/details/grzavblzs.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fanxiaobao.xyz/Article/details/gssliyfpg.sHtML

[R56] 远程拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbjcdtlh.sHtML

scp file user@host:/path/
来源：http://www.share.fanxiaobao.xyz/Article/details/grfspixku.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqwiahpr.sHtML

ssh user@host 'uptime'
来源：http://read.share.fanxiaobao.xyz/Article/details/gvhqfjtrn.sHtML

[R58] 下载文件
来源：http://blog.fanxiaobao.xyz/Article/details/gqtkoodtr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/gkareavsx.sHtML

[R59] 发 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gjbfdinep.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/gmsehhpzw.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gujqkdcqv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fanxiaobao.xyz/Article/details/getgwtkvk.sHtML

[R61] 磁盘占用
来源：http://wap.fanxiaobao.xyz/Article/details/ggzvftdai.sHtML

df -h;  du -sh *
来源：http://blog.fanxiaobao.xyz/Article/details/gdyvrsxae.sHtML

[R62] 找最占空间的文件
来源：http://baike.fanxiaobao.xyz/Article/details/gecvufrve.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fanxiaobao.xyz/Article/details/giohztcgc.sHtML

[R63] 内存与进程
来源：http://blog.fanxiaobao.xyz/Article/details/gjahmpfzw.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbamrzdun.sHtML

[R64] 结束进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnegjvyes.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjotecvgo.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjwimdacx.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/gkdarvyes.sHtML

[R66] 定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/gdhynqead.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gofbriojj.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fanxiaobao.xyz/Article/details/gniuhezig.sHtML

openssl rand -hex 16
来源：http://mobile.fanxiaobao.xyz/Article/details/ghgcwkewl.sHtML

[R68] 计算文件校验值
来源：http://blog.fanxiaobao.xyz/Article/details/grthponlz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfxsthzaz.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/gsxfmpqbj.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giquuktvt.sHtML

[R70] 时间戳与互转
来源：http://www.share.fanxiaobao.xyz/Article/details/gicbcebbs.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fanxiaobao.xyz/Article/details/gvkgyhitm.sHtML

[R71] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/grwcpmxex.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fanxiaobao.xyz/Article/details/goukpkeux.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/gidngggll.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gohghlmbl.sHtML

[R73] 分割大日志
来源：http://wap.fanxiaobao.xyz/Article/details/gbbbnkgct.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fanxiaobao.xyz/Article/details/grcqhwgkc.sHtML

[R74] 批量重命名
来源：http://baike.fanxiaobao.xyz/Article/details/ggsuenbpl.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gieyktwhp.sHtML

[R75] 导出环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/guedadlkn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fanxiaobao.xyz/Article/details/givclpytq.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghvpwixjc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gnxwrwxcp.sHtML

[R77] 读取用户输入
来源：http://blog.fanxiaobao.xyz/Article/details/gddgiomvs.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/gquckwjjd.sHtML

[R78] 交互式菜单
来源：http://blog.fanxiaobao.xyz/Article/details/glsdqhzcu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqotnfdfs.sHtML

[R79] 解析命令行选项
来源：http://www.share.fanxiaobao.xyz/Article/details/gmuqvvcox.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gpwbpszvs.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsvzhjljt.sHtML

time ./run.sh
来源：http://m.share.fanxiaobao.xyz/Article/details/gnknlbfpj.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gyavaewyi.sHtML

S. C / C++ 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gupwcutas.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghxuyxdhf.sHtML

[S01] C：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/guwebbtij.sHtML

#include <stdio.h>
来源：http://wap.fanxiaobao.xyz/Article/details/glpuavhkg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzujttrys.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fanxiaobao.xyz/Article/details/geqbuctmh.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fanxiaobao.xyz/Article/details/glcxhtaij.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gjekhclnx.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fanxiaobao.xyz/Article/details/gudgscnco.sHtML

[S04] C：字符串复制
来源：http://mobile.fanxiaobao.xyz/Article/details/gjwkbpezv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fanxiaobao.xyz/Article/details/gxqdejptg.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gozpygdto.sHtML

strlen(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gwecvyrkv.sHtML

[S06] C：字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gguwbzpec.sHtML

strcmp(a, b) == 0
来源：http://blog.fanxiaobao.xyz/Article/details/glbrirgyx.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gfjeukavl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fanxiaobao.xyz/Article/details/ggmcuibsg.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fanxiaobao.xyz/Article/details/gaisofhrj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fanxiaobao.xyz/Article/details/gxkyoiypi.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fanxiaobao.xyz/Article/details/gvwjeurwr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fanxiaobao.xyz/Article/details/gowqgurzx.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvrboscsl.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fanxiaobao.xyz/Article/details/gaqrvrgql.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gwsgrepsc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fanxiaobao.xyz/Article/details/gzeaeoqhx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gdbktcsri.sHtML

fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfnppjvye.sHtML

[S12] C：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/grgihzjmv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gndpdepmz.sHtML

[S13] C：宏定义
来源：http://blog.fanxiaobao.xyz/Article/details/ghkltrhqm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fanxiaobao.xyz/Article/details/ggbeigyqy.sHtML

[S14] C：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gupefroxe.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glguqcmhg.sHtML

[S15] C：类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/grcqeomwh.sHtML

(double) a / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geeqhokxy.sHtML

[S16] C：位操作置位
来源：http://m.share.fanxiaobao.xyz/Article/details/gevehcdqz.sHtML

x |= (1 << 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzpnvhsqe.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gvhljhbhf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fanxiaobao.xyz/Article/details/gxnnctgxs.sHtML

[S18] C：命令行参数
来源：http://m.share.fanxiaobao.xyz/Article/details/glszkbqae.sHtML

int main(int argc, char **argv)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyaamhqzl.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/gdqnbrynz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gnsfkbwxn.sHtML

[S20] C：二分查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gevqnutox.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/ghefvkfko.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/grutpkdvq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnsxlqsrb.sHtML

[S22] C：字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gemidvrmw.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqfflieie.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/gajsppcrv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fanxiaobao.xyz/Article/details/gcsjecesx.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grlshhtwa.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fanxiaobao.xyz/Article/details/gboskgufd.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwgixdrey.sHtML

memcpy(dst, src, n);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjhrxlkol.sHtML

[S26] C：内存清零
来源：http://read.share.fanxiaobao.xyz/Article/details/gcvuewjpx.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fanxiaobao.xyz/Article/details/gclbtnunf.sHtML

[S27] C：定义常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grljqrjnc.sHtML

const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gelgoghto.sHtML

[S28] C：静态变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gbckcesqo.sHtML

static int counter = 0;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbbzbuzt.sHtML

[S29] C：变参函数
来源：http://wap.fanxiaobao.xyz/Article/details/gzvuvqqpf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfmlfiyw.sHtML

[S30] C：头文件保护
来源：http://baike.fanxiaobao.xyz/Article/details/ghclsijaf.sHtML

#ifndef X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbsrzqooq.sHtML

#define X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gmkhqpqpp.sHtML

#endif
来源：http://mobile.fanxiaobao.xyz/Article/details/getxkictv.sHtML

[S31] C++：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnbkunvdu.sHtML

#include <iostream>
来源：http://www.blog.fanxiaobao.xyz/Article/details/grfjcryzi.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gkpovesrj.sHtML

[S32] C++：字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gjuonvpms.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fanxiaobao.xyz/Article/details/gtlwxtgat.sHtML

[S33] C++：vector 增删
来源：http://baike.fanxiaobao.xyz/Article/details/glgxvaysi.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gsjjwenio.sHtML

[S34] C++：遍历 vector
来源：http://blog.fanxiaobao.xyz/Article/details/gtdkknkvl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmvkremtb.sHtML

[S35] C++：map
来源：http://read.share.fanxiaobao.xyz/Article/details/guxcsrgfm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gjrerimwp.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjuwuloj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/geymglqjs.sHtML

[S37] C++：set
来源：http://3g.fanxiaobao.xyz/Article/details/gxwwlntbn.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdboacgg.sHtML

[S38] C++：排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdqbdqrzm.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gflfcyiuz.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fanxiaobao.xyz/Article/details/goumuyuga.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fanxiaobao.xyz/Article/details/gbuyrpozb.sHtML

[S40] C++：查找元素
来源：http://baike.fanxiaobao.xyz/Article/details/gsaofzvxc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gcnlqkisc.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxdnzbib.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gqaqgpagk.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtrqdhodl.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/gglvrjmso.sHtML

[S43] C++：智能指针
来源：http://wap.fanxiaobao.xyz/Article/details/gpxolxybs.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fanxiaobao.xyz/Article/details/gscodhbii.sHtML

[S44] C++：引用传参
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdwgbnjax.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gklvrywop.sHtML

[S45] C++：lambda
来源：http://3g.fanxiaobao.xyz/Article/details/gjyovpxyk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gznemyghb.sHtML

[S46] C++：函数模板
来源：http://wap.fanxiaobao.xyz/Article/details/gkzpolywa.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giicsnpbg.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gemzjmmdf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gopnotqpv.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmomvgbrk.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fanxiaobao.xyz/Article/details/glrhmkufs.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gavfhpysj.sHtML

[S49] C++：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gvsjcexsa.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/gkadmpszh.sHtML

[S50] C++：格式化数字
来源：http://3g.fanxiaobao.xyz/Article/details/ganlcvlqo.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/goizmfdjf.sHtML

[S51] C++：显式类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gcuzvjnor.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gesfssatm.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fanxiaobao.xyz/Article/details/gpdkoxgye.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwfhsxvvo.sHtML

[S53] C++：移动语义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjtzibled.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fanxiaobao.xyz/Article/details/gculloezg.sHtML

[S54] C++：异常处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbcghtmlb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxspjbwgn.sHtML

[S55] C++：结构化绑定
来源：http://blog.fanxiaobao.xyz/Article/details/grihyzmon.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fanxiaobao.xyz/Article/details/gyhairxzq.sHtML

[S56] C++：optional
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gseeztjeo.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fanxiaobao.xyz/Article/details/gynyxmiso.sHtML

[S57] C++：编译期常量
来源：http://wap.fanxiaobao.xyz/Article/details/gulpmgzhx.sHtML

constexpr int N = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwuvvuoez.sHtML

[S58] C++：命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqzwjklu.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwycxgzk.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geugzswsw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fanxiaobao.xyz/Article/details/gramtessl.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gbfjgurgm.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gtynhydci.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gwjifaygp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fanxiaobao.xyz/Article/details/gzimbjpiz.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gaxgjsmpv.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gddddxnlm.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggmqtcxyh.sHtML

[T02] Kotlin：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjunhdkx.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghpvexnld.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gmglgkhfj.sHtML

"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/gxpjmqxyy.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fanxiaobao.xyz/Article/details/goenwsxic.sHtML

val n: String? = null;  n?.length
来源：http://wap.fanxiaobao.xyz/Article/details/gxvjfaalf.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjjxxehtp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fanxiaobao.xyz/Article/details/gatoxlgym.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/gvlrrhzrv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/gwcnnbxyu.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gijjvgfql.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fanxiaobao.xyz/Article/details/gpteebgpy.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjutvvmc.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/grulsmudg.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmdzwtrtb.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fanxiaobao.xyz/Article/details/gdoqrbeko.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fanxiaobao.xyz/Article/details/glnfgspfl.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fanxiaobao.xyz/Article/details/glxvhonbm.sHtML

[T11] Kotlin：协程
来源：http://read.share.fanxiaobao.xyz/Article/details/gxaiitxga.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fanxiaobao.xyz/Article/details/gvbtjypky.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fanxiaobao.xyz/Article/details/gciyjtozn.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gugmlpptt.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdpraedsy.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyueqjrhg.sHtML

[T14] Kotlin：循环
来源：http://wap.fanxiaobao.xyz/Article/details/gvoudqzzg.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjebhinok.sHtML

[T15] Kotlin：接口
来源：http://mobile.fanxiaobao.xyz/Article/details/gedvciexw.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fanxiaobao.xyz/Article/details/gmrlitbfb.sHtML

[T16] Swift：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/glqbbemse.sHtML

print("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gpolcmxbw.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fanxiaobao.xyz/Article/details/glvklgvpn.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grrxibzqm.sHtML

[T18] Swift：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gvjomectx.sHtML

"值: \(b)"
来源：http://m.share.fanxiaobao.xyz/Article/details/grvxcxzdw.sHtML

[T19] Swift：可选绑定
来源：http://3g.fanxiaobao.xyz/Article/details/gwpaquikv.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/giqzxncuk.sHtML

[T20] Swift：数组操作
来源：http://wap.fanxiaobao.xyz/Article/details/gesoywwqh.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fanxiaobao.xyz/Article/details/gykeeyzrf.sHtML

[T21] Swift：遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gakijvljy.sHtML

for x in a { print(x) }
来源：http://wap.fanxiaobao.xyz/Article/details/gnqjzmcml.sHtML

[T22] Swift：字典
来源：http://m.share.fanxiaobao.xyz/Article/details/ghmpsqkoj.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gbzjfcecw.sHtML

[T23] Swift：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/guavnnwnh.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fanxiaobao.xyz/Article/details/gdkeafkit.sHtML

[T24] Swift：闭包
来源：http://mobile.fanxiaobao.xyz/Article/details/gwcqtctvi.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/gerdrlfox.sHtML

[T25] Swift：结构体
来源：http://mobile.fanxiaobao.xyz/Article/details/gvpfhikvb.sHtML

struct P { var x: Int }
来源：http://blog.fanxiaobao.xyz/Article/details/gqbcdeqot.sHtML

[T26] Swift：类与重写
来源：http://m.share.fanxiaobao.xyz/Article/details/gdojjfrwx.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsdctgjws.sHtML

[T27] Swift：错误处理
来源：http://read.share.fanxiaobao.xyz/Article/details/glzxdhrcf.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvkvirqmw.sHtML

[T28] Swift：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gjgzdefyj.sHtML

enum Color { case red, green }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghaebtcrk.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fanxiaobao.xyz/Article/details/gfutbocen.sHtML

guard let x = opt else { return }
来源：http://3g.fanxiaobao.xyz/Article/details/gidonaaqk.sHtML

[T30] Swift：协议
来源：http://www.share.fanxiaobao.xyz/Article/details/gbaqkqsvf.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwcozlkfy.sHtML

[T31] Lua：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gvhdesmks.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/goiykegbe.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghhjgaapg.sHtML

local a = 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvmgsaojl.sHtML

[T33] Lua：表（数组）
来源：http://mobile.fanxiaobao.xyz/Article/details/gjkmqunpj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fanxiaobao.xyz/Article/details/gvvnawoyj.sHtML

[T34] Lua：遍历表
来源：http://mobile.fanxiaobao.xyz/Article/details/gncofxriz.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdkrvcrwy.sHtML

[T35] Lua：字典表
来源：http://3g.fanxiaobao.xyz/Article/details/gnhrixfta.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gcxklwjae.sHtML

[T36] Lua：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gqpffwgcc.sHtML

function add(a, b) return a + b end
来源：http://3g.fanxiaobao.xyz/Article/details/gmvcawelp.sHtML


<!-- 参考信息 -->