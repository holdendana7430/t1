代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gfjcmrisr.sHtML

[R32] 参数个数校验
来源：http://3g.fanxiaobao.xyz/Article/details/gjxikceux.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gawuzswdx.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gahavoutb.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fanxiaobao.xyz/Article/details/ggrzmhcmz.sHtML

[R34] 退出时清理
来源：http://www.share.fanxiaobao.xyz/Article/details/guvzgsqlw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjxjirsin.sHtML

[R35] 后台执行并等待
来源：http://3g.fanxiaobao.xyz/Article/details/gxnvulyux.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gimjdnlho.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gcucdoxdx.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fanxiaobao.xyz/Article/details/gulrjvwht.sHtML

[R37] 把输出赋给变量
来源：http://3g.fanxiaobao.xyz/Article/details/gujvattfi.sHtML

files=$(ls -1)
来源：http://baike.fanxiaobao.xyz/Article/details/gsfcnkfjt.sHtML

[R38] 管道串联
来源：http://wap.fanxiaobao.xyz/Article/details/gkirkvlvw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gofjmvemb.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fanxiaobao.xyz/Article/details/gqsjhwehf.sHtML

cmd > out.log 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gtgbbzffw.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjpcvvdzh.sHtML

echo "log" >> out.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gajgmxmdi.sHtML

[R41] 丢弃输出
来源：http://wap.fanxiaobao.xyz/Article/details/grinxnmyq.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gaoqwuhdi.sHtML

[R42] 输入重定向
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghsqeklxb.sHtML

wc -l < a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gatxdfvmr.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbxyyntfy.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gbnkzhbzg.sHtML

[R44] 按修改时间查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gbsnozaua.sHtML

find . -mtime -7 -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gezrexeho.sHtML

[R45] 批量删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwgnzhvi.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fanxiaobao.xyz/Article/details/gjffqlsti.sHtML

[R46] 递归替换文件内容
来源：http://wap.fanxiaobao.xyz/Article/details/gwcdugkzh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fanxiaobao.xyz/Article/details/gcriupucr.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gbfhvdchv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjjeongve.sHtML

[R48] awk 取指定列
来源：http://www.share.fanxiaobao.xyz/Article/details/gwurufbce.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gghizdbkd.sHtML

[R49] awk 带条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glltbvdsd.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/gzmmritqs.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gblzdzglc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvytmjytg.sHtML

[R51] 排序去重取前几
来源：http://blog.fanxiaobao.xyz/Article/details/gzkahxwfe.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/gznjcrueg.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/giliumrvq.sHtML

wc -l a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtorpvhrd.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fanxiaobao.xyz/Article/details/gizjgrmrq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fanxiaobao.xyz/Article/details/gsmekhfdv.sHtML

[R54] 比较两个文件
来源：http://wap.fanxiaobao.xyz/Article/details/gzuadpsjo.sHtML

diff a.txt b.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gdysxwfjv.sHtML

[R55] 压缩与解压
来源：http://mobile.fanxiaobao.xyz/Article/details/ghgycbfhk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fanxiaobao.xyz/Article/details/gzdfxowcg.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gvzphkkli.sHtML

scp file user@host:/path/
来源：http://baike.fanxiaobao.xyz/Article/details/gbwuitgfs.sHtML

[R57] 远程执行命令
来源：http://blog.fanxiaobao.xyz/Article/details/gjcxoimqc.sHtML

ssh user@host 'uptime'
来源：http://www.share.fanxiaobao.xyz/Article/details/gicdhokwi.sHtML

[R58] 下载文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gcrkwvllj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fanxiaobao.xyz/Article/details/gfjirzpeg.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkptnegsw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/gxcxinhue.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gbsuvaurl.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gdrlsocyo.sHtML

[R61] 磁盘占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gxuuhdkki.sHtML

df -h;  du -sh *
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtuydeozf.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjilpxpnw.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjxpsqty.sHtML

[R63] 内存与进程
来源：http://3g.fanxiaobao.xyz/Article/details/gmxrpzetz.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fanxiaobao.xyz/Article/details/gsbtcwdlq.sHtML

[R64] 结束进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gidmgmqll.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fanxiaobao.xyz/Article/details/gsifrlshw.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gknaiwfpe.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fanxiaobao.xyz/Article/details/giinverxm.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gszukvwwo.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixyhtgan.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fanxiaobao.xyz/Article/details/gzavqhxhh.sHtML

openssl rand -hex 16
来源：http://3g.fanxiaobao.xyz/Article/details/gwlijbtsk.sHtML

[R68] 计算文件校验值
来源：http://3g.fanxiaobao.xyz/Article/details/gbxfodqqr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gzvcjiwdl.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glaziinqz.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fanxiaobao.xyz/Article/details/gmtcdksds.sHtML

[R70] 时间戳与互转
来源：http://www.share.fanxiaobao.xyz/Article/details/gnpdlbrco.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fanxiaobao.xyz/Article/details/gmbimhqtn.sHtML

[R71] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gwqdpvgis.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fanxiaobao.xyz/Article/details/gtdgbpsuc.sHtML

[R72] 等待端口就绪
来源：http://3g.fanxiaobao.xyz/Article/details/gaczmbmxw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gefdqyiiv.sHtML

[R73] 分割大日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggtzkcpkp.sHtML

split -l 1000 big.log part_
来源：http://wap.fanxiaobao.xyz/Article/details/grwomkrva.sHtML

[R74] 批量重命名
来源：http://read.share.fanxiaobao.xyz/Article/details/guftzsfll.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gocfydauc.sHtML

[R75] 导出环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gpzlvjduw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fanxiaobao.xyz/Article/details/gemgkimvb.sHtML

[R76] 使用临时文件
来源：http://mobile.fanxiaobao.xyz/Article/details/guyndqnyp.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/ggyxafjpd.sHtML

[R77] 读取用户输入
来源：http://3g.fanxiaobao.xyz/Article/details/grphhalho.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghqweasli.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/gjketcdwu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fanxiaobao.xyz/Article/details/gihfphkhq.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaztforrm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fanxiaobao.xyz/Article/details/geteunqpe.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fanxiaobao.xyz/Article/details/gfhlyjbre.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/gixobevos.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcjumrdbf.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gdaaqpmsm.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gxffmjvtr.sHtML

[S01] C：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gimxmowel.sHtML

#include <stdio.h>
来源：http://mobile.fanxiaobao.xyz/Article/details/gnygxfgli.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fanxiaobao.xyz/Article/details/gaiwmsbkp.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gurdrxcvo.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fanxiaobao.xyz/Article/details/gsxkeohof.sHtML

[S03] C：读入整数
来源：http://blog.fanxiaobao.xyz/Article/details/gzcfoxdrq.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glieapsfl.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmtkiuygs.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyogllenc.sHtML

[S05] C：字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gkeexlhgh.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gwtlzpjzc.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glasexbds.sHtML

strcmp(a, b) == 0
来源：http://www.share.fanxiaobao.xyz/Article/details/gajtwxypp.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gvciugdxz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fanxiaobao.xyz/Article/details/gvitbwfex.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fanxiaobao.xyz/Article/details/gswjohttp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fanxiaobao.xyz/Article/details/gvokqrfvt.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fanxiaobao.xyz/Article/details/ghzpevwrn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fanxiaobao.xyz/Article/details/guvaeooml.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/gdivgzeem.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggfofzdin.sHtML

[S11] C：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgfdafud.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fanxiaobao.xyz/Article/details/godpclxcr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geefgwxbk.sHtML

fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfjoualqs.sHtML

[S12] C：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gighsamhz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghloaibpq.sHtML

[S13] C：宏定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gdrcwlnlg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcytssgcv.sHtML

[S14] C：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goyyatgmd.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fanxiaobao.xyz/Article/details/gnsfzspbj.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gifqoyesw.sHtML

(double) a / b
来源：http://wap.fanxiaobao.xyz/Article/details/gqxzbxeyz.sHtML

[S16] C：位操作置位
来源：http://3g.fanxiaobao.xyz/Article/details/gtlfldgsx.sHtML

x |= (1 << 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gcwsrgiwn.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/goqtmcvnw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fanxiaobao.xyz/Article/details/gwbegvjrx.sHtML

[S18] C：命令行参数
来源：http://3g.fanxiaobao.xyz/Article/details/gjuakrlfw.sHtML

int main(int argc, char **argv)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbpzwvdtm.sHtML

[S19] C：快速排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gcpgngteb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gwvnhrjxf.sHtML

[S20] C：二分查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gphgtkomd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gvdeycxxu.sHtML

[S21] C：字符类别判断
来源：http://wap.fanxiaobao.xyz/Article/details/gvusyqdbf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/gctfrrolk.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggfhjsoum.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgbwhejr.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/gokytwtcr.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/glsbrvmty.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geynnqney.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fanxiaobao.xyz/Article/details/gkbhvygtm.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gaapnrppl.sHtML

memcpy(dst, src, n);
来源：http://www.share.fanxiaobao.xyz/Article/details/gymnopeum.sHtML

[S26] C：内存清零
来源：http://baike.fanxiaobao.xyz/Article/details/gevcanmzk.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gyxalvoil.sHtML

[S27] C：定义常量
来源：http://baike.fanxiaobao.xyz/Article/details/gqlnwpxom.sHtML

const double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gemcohnol.sHtML

[S28] C：静态变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbvqzocim.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbykhxpnc.sHtML

[S29] C：变参函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gubhxragx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmaetdbzm.sHtML

[S30] C：头文件保护
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcjekwvwh.sHtML

#ifndef X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gfomhwenj.sHtML

#define X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gebbbeygp.sHtML

#endif
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmfthotgd.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gognxaylu.sHtML

#include <iostream>
来源：http://m.share.fanxiaobao.xyz/Article/details/gkjlzfnno.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gxfnrzvzb.sHtML

[S32] C++：字符串
来源：http://3g.fanxiaobao.xyz/Article/details/glvqkjfnq.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fanxiaobao.xyz/Article/details/grsqhifnf.sHtML

[S33] C++：vector 增删
来源：http://baike.fanxiaobao.xyz/Article/details/gphboohyx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fanxiaobao.xyz/Article/details/grxgjoadf.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fanxiaobao.xyz/Article/details/gvqtwleyx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmufpsnf.sHtML

[S35] C++：map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvrrwfwxu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gyeumscqu.sHtML

[S36] C++：unordered_map
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbumeonx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gysaisxwj.sHtML

[S37] C++：set
来源：http://baike.fanxiaobao.xyz/Article/details/gzjbrxfor.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gepgbslgg.sHtML

[S38] C++：排序
来源：http://mobile.fanxiaobao.xyz/Article/details/ggmdivuvi.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gkuybmxgx.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fanxiaobao.xyz/Article/details/gmqzgcplx.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fanxiaobao.xyz/Article/details/gdvcdejmq.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gdqzklrbd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/guesrcqhp.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmgwvnbc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvkxczzjn.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fanxiaobao.xyz/Article/details/givrzofwh.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fanxiaobao.xyz/Article/details/giwnvsofy.sHtML

[S43] C++：智能指针
来源：http://mobile.fanxiaobao.xyz/Article/details/gtqrcxupv.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwsvoqhw.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozawawtt.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gudedofac.sHtML

[S45] C++：lambda
来源：http://mobile.fanxiaobao.xyz/Article/details/gshpvutyr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzqnhjbha.sHtML

[S46] C++：函数模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gptdbzxbv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcsvghdda.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gfqgzjjff.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grmqoghkg.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdriivanq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gedsvtrhb.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gxyfhlcbk.sHtML

[S49] C++：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/grrltrdan.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gwzsjcnkv.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyunpcbcy.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gofnolixu.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/guaoawhaf.sHtML

static_cast<double>(a) / b
来源：http://mobile.fanxiaobao.xyz/Article/details/guvwwhpfm.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fanxiaobao.xyz/Article/details/ghadgqjpn.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fanxiaobao.xyz/Article/details/gvjabtszg.sHtML

[S53] C++：移动语义
来源：http://baike.fanxiaobao.xyz/Article/details/ggpbhjdib.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fanxiaobao.xyz/Article/details/gfwrvfags.sHtML

[S54] C++：异常处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gbdoddmmu.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjuezmiff.sHtML

[S55] C++：结构化绑定
来源：http://wap.fanxiaobao.xyz/Article/details/gdyuxprye.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghlcppjxe.sHtML

[S56] C++：optional
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsnmduxcc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdwfbdgm.sHtML

[S57] C++：编译期常量
来源：http://baike.fanxiaobao.xyz/Article/details/goeuhksrr.sHtML

constexpr int N = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gveuxxblt.sHtML

[S58] C++：命名空间
来源：http://wap.fanxiaobao.xyz/Article/details/gqwxtzysl.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/griegpnng.sHtML

[S59] C++：静态断言
来源：http://www.share.fanxiaobao.xyz/Article/details/giairlhzc.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fanxiaobao.xyz/Article/details/gxastqyqu.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fanxiaobao.xyz/Article/details/gyvedslyf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gzrxevyvi.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gddkzjuwk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gulrlwber.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/ghgosadtj.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gegniaiea.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gwffaptmc.sHtML

[T02] Kotlin：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gaudhgzom.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glshngktp.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fanxiaobao.xyz/Article/details/gyqjggfis.sHtML

"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gbntbcpqe.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fanxiaobao.xyz/Article/details/gvafghwlc.sHtML

val n: String? = null;  n?.length
来源：http://3g.fanxiaobao.xyz/Article/details/gkcffiomv.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gyacggdom.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fanxiaobao.xyz/Article/details/glgqmamkq.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/gikcfyheg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjylpfjpg.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fanxiaobao.xyz/Article/details/grlctewee.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fanxiaobao.xyz/Article/details/gzftmiqnm.sHtML

[T08] Kotlin：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/gadveculu.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjpzdmdqq.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcfihropd.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxsxbqpo.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjvxzjse.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fanxiaobao.xyz/Article/details/gobycanui.sHtML

[T11] Kotlin：协程
来源：http://3g.fanxiaobao.xyz/Article/details/gfoaxpflv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fanxiaobao.xyz/Article/details/gbwyklsfw.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fanxiaobao.xyz/Article/details/gkdnatfys.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqzqkvgqh.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fanxiaobao.xyz/Article/details/gqbouygwa.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gydqlwimv.sHtML

[T14] Kotlin：循环
来源：http://3g.fanxiaobao.xyz/Article/details/ghfiuegvb.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdxykjyrp.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaqwqtsef.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjletzmhm.sHtML

[T16] Swift：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gxelxwahf.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gniedmfyu.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdhftngt.sHtML

var a = 1;  let b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gqhdpaptc.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkxjhfmpr.sHtML

"值: \(b)"
来源：http://read.share.fanxiaobao.xyz/Article/details/gqiqaxikc.sHtML

[T19] Swift：可选绑定
来源：http://3g.fanxiaobao.xyz/Article/details/gvmvldkoo.sHtML

if let n = opt { print(n) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpqqfvrib.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwpstlgew.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fanxiaobao.xyz/Article/details/glivejccz.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwnnnjwt.sHtML

for x in a { print(x) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvzqxnnls.sHtML

[T22] Swift：字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtwjcurlv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gdangzcup.sHtML

[T23] Swift：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gppljfglw.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfltmzsda.sHtML

[T24] Swift：闭包
来源：http://wap.fanxiaobao.xyz/Article/details/gjkeyfozm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gadlamxgc.sHtML

[T25] Swift：结构体
来源：http://wap.fanxiaobao.xyz/Article/details/gpglnxfcc.sHtML

struct P { var x: Int }
来源：http://baike.fanxiaobao.xyz/Article/details/gxadlfusc.sHtML

[T26] Swift：类与重写
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwmouomw.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fanxiaobao.xyz/Article/details/gigefdrdl.sHtML

[T27] Swift：错误处理
来源：http://wap.fanxiaobao.xyz/Article/details/gwlijlucg.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdbwkhsxl.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbkfcfusq.sHtML

enum Color { case red, green }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbtaoywn.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fanxiaobao.xyz/Article/details/gjqjlwwot.sHtML

guard let x = opt else { return }
来源：http://3g.fanxiaobao.xyz/Article/details/gnmznbsio.sHtML

[T30] Swift：协议
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmethkdhc.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpqckyzoe.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gotwtwbrw.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gmbkdhfhw.sHtML

[T32] Lua：局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbsjnjluj.sHtML

local a = 1
来源：http://m.share.fanxiaobao.xyz/Article/details/ghaajapiv.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fanxiaobao.xyz/Article/details/goytjuapm.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.fanxiaobao.xyz/Article/details/gzuaylzef.sHtML

[T34] Lua：遍历表
来源：http://baike.fanxiaobao.xyz/Article/details/grxwjltoo.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.fanxiaobao.xyz/Article/details/gmxsaneff.sHtML


<!-- 参考信息 -->