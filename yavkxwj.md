代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fanxiaobao.xyz/Article/details/grsjnpmvr.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsdxkwhcj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvkzrmytq.sHtML

[R37] 把输出赋给变量
来源：http://blog.fanxiaobao.xyz/Article/details/gvbvmcuft.sHtML

files=$(ls -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gupdcgyvt.sHtML

[R38] 管道串联
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzlinaof.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fanxiaobao.xyz/Article/details/gwqepuasl.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkreutake.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxpyiafi.sHtML

[R40] 追加写日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gflqzhxvz.sHtML

echo "log" >> out.log
来源：http://3g.fanxiaobao.xyz/Article/details/gmnbaotfy.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/gqxljxgdn.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gcfkqakwf.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/guiexbdrv.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghpsvowdj.sHtML

[R43] 按名字查找文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gxrhczdnk.sHtML

find . -name "*.log" -type f
来源：http://baike.fanxiaobao.xyz/Article/details/glsuqbxjc.sHtML

[R44] 按修改时间查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gonakglnr.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcyahnxqn.sHtML

[R45] 批量删除
来源：http://m.share.fanxiaobao.xyz/Article/details/gdeoabqsd.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fanxiaobao.xyz/Article/details/gvxuclpak.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmjbpztxl.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/gtajarbro.sHtML

[R47] sed 单行替换
来源：http://blog.fanxiaobao.xyz/Article/details/gpiklltlq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/glveqngjx.sHtML

[R48] awk 取指定列
来源：http://blog.fanxiaobao.xyz/Article/details/giuwibjys.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gawgltqed.sHtML

[R49] awk 带条件
来源：http://blog.fanxiaobao.xyz/Article/details/gyyoadlxw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fanxiaobao.xyz/Article/details/gfdaszaze.sHtML

[R50] awk 求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjhisleu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gefgdmoah.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/goxvahpps.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fanxiaobao.xyz/Article/details/gozosmwgq.sHtML

[R52] 统计行数
来源：http://read.share.fanxiaobao.xyz/Article/details/gjltzjqze.sHtML

wc -l a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gnuuicenv.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fanxiaobao.xyz/Article/details/gzwrwsgnb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/glkjpjlmh.sHtML

[R54] 比较两个文件
来源：http://wap.fanxiaobao.xyz/Article/details/goajczijd.sHtML

diff a.txt b.txt
来源：http://baike.fanxiaobao.xyz/Article/details/glygnulki.sHtML

[R55] 压缩与解压
来源：http://3g.fanxiaobao.xyz/Article/details/gnbgkqbpw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fanxiaobao.xyz/Article/details/gbqhckndz.sHtML

[R56] 远程拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gccqjocha.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/gorzflnwh.sHtML

[R57] 远程执行命令
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxibvizr.sHtML

ssh user@host 'uptime'
来源：http://www.share.fanxiaobao.xyz/Article/details/gprtmsdmr.sHtML

[R58] 下载文件
来源：http://wap.fanxiaobao.xyz/Article/details/geesqfkib.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fanxiaobao.xyz/Article/details/grinufsnv.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guayndmfx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/gqfofxnzc.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gzcghnlnf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gdiedomht.sHtML

[R61] 磁盘占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gylcpxlhu.sHtML

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/gizdohfnx.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfiveqwyn.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fanxiaobao.xyz/Article/details/gmyjzdpty.sHtML

[R63] 内存与进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbkxoqwfo.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmmtuzgh.sHtML

[R64] 结束进程
来源：http://3g.fanxiaobao.xyz/Article/details/gokxegqtg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsjvcxwxc.sHtML

[R65] 查看端口占用
来源：http://read.share.fanxiaobao.xyz/Article/details/grggvwrmk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fanxiaobao.xyz/Article/details/glmqsbmsi.sHtML

[R66] 定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gzwoumbjo.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzqwzhhuz.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fanxiaobao.xyz/Article/details/gmpylrkko.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/gtqzlthzj.sHtML

[R68] 计算文件校验值
来源：http://3g.fanxiaobao.xyz/Article/details/gtsvattji.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gijsswhgs.sHtML

[R69] 生成随机密码
来源：http://blog.fanxiaobao.xyz/Article/details/gpjwttakt.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fanxiaobao.xyz/Article/details/gmuyjntdd.sHtML

[R70] 时间戳与互转
来源：http://baike.fanxiaobao.xyz/Article/details/goswitxsy.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyrhmrllh.sHtML

[R71] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbfxrbyx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fanxiaobao.xyz/Article/details/gjqbyrwah.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gugziseiw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/grsesqqih.sHtML

[R73] 分割大日志
来源：http://wap.fanxiaobao.xyz/Article/details/gppexfwpu.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcbsmusll.sHtML

[R74] 批量重命名
来源：http://mobile.fanxiaobao.xyz/Article/details/gnonmkmhu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gaoaylrkf.sHtML

[R75] 导出环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gpdicdhwm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fanxiaobao.xyz/Article/details/gvnaqnqyx.sHtML

[R76] 使用临时文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gpokhctuu.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkovobruy.sHtML

[R77] 读取用户输入
来源：http://mobile.fanxiaobao.xyz/Article/details/gecfotqdf.sHtML

read -rp "请输入: " ans
来源：http://www.share.fanxiaobao.xyz/Article/details/gjqijptbe.sHtML

[R78] 交互式菜单
来源：http://mobile.fanxiaobao.xyz/Article/details/girpbsgjt.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fanxiaobao.xyz/Article/details/gmijmyshr.sHtML

[R79] 解析命令行选项
来源：http://3g.fanxiaobao.xyz/Article/details/gdrfhjyib.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fanxiaobao.xyz/Article/details/gcbsdbsld.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/gzislyjqs.sHtML

time ./run.sh
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxvcxpemv.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwyldlqpq.sHtML

S. C / C++ 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gllboofrr.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gzirauosg.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gklmplgja.sHtML

#include <stdio.h>
来源：http://baike.fanxiaobao.xyz/Article/details/gbwbqdhhy.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fanxiaobao.xyz/Article/details/ggpmzoqbq.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/gyvrhnhax.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fanxiaobao.xyz/Article/details/gnsvvkuyq.sHtML

[S03] C：读入整数
来源：http://baike.fanxiaobao.xyz/Article/details/gzhecwzgn.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grigghyme.sHtML

[S04] C：字符串复制
来源：http://mobile.fanxiaobao.xyz/Article/details/gmvujlkzi.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/gvvdbyvhi.sHtML

[S05] C：字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gjreqfskb.sHtML

strlen(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gipjtbbge.sHtML

[S06] C：字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtqgtahvt.sHtML

strcmp(a, b) == 0
来源：http://m.share.fanxiaobao.xyz/Article/details/gxfxqlryv.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gibalgugc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggsvzsvcb.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzwxddoky.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fanxiaobao.xyz/Article/details/gidrumemc.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzfsmznlq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fanxiaobao.xyz/Article/details/gttlbscqo.sHtML

[S10] C：指针与解引用
来源：http://read.share.fanxiaobao.xyz/Article/details/gnhtsnksn.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqixbpbmx.sHtML

[S11] C：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gdbehnjkf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fanxiaobao.xyz/Article/details/gdvvglkam.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmkezttb.sHtML

fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grigztlcy.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gduhkikwl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyyenipwr.sHtML

[S13] C：宏定义
来源：http://read.share.fanxiaobao.xyz/Article/details/ggyxlvftf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fanxiaobao.xyz/Article/details/gnrpsdysx.sHtML

[S14] C：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/giozgypyc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fanxiaobao.xyz/Article/details/giuiyldym.sHtML

[S15] C：类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gscwzykzp.sHtML

(double) a / b
来源：http://baike.fanxiaobao.xyz/Article/details/givnobule.sHtML

[S16] C：位操作置位
来源：http://m.share.fanxiaobao.xyz/Article/details/gziaamzxj.sHtML

x |= (1 << 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxdtkapn.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzvclxds.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdtdncrox.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gtmcxcqsz.sHtML

int main(int argc, char **argv)
来源：http://blog.fanxiaobao.xyz/Article/details/gllfvcanh.sHtML

[S19] C：快速排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gaeqfrowo.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gxzpuejfx.sHtML

[S20] C：二分查找
来源：http://wap.fanxiaobao.xyz/Article/details/gcgtfiuls.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gugwrypxv.sHtML

[S21] C：字符类别判断
来源：http://m.share.fanxiaobao.xyz/Article/details/ghauyagnr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fanxiaobao.xyz/Article/details/glizkfrpg.sHtML

[S22] C：字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/ggdwihaej.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fanxiaobao.xyz/Article/details/gktilpzvp.sHtML

[S23] C：随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/guxyzxmxw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gkvhmkubt.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/gytzahylp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fanxiaobao.xyz/Article/details/gzxuhpbkz.sHtML

[S25] C：内存拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhrncbip.sHtML

memcpy(dst, src, n);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxbowjawj.sHtML

[S26] C：内存清零
来源：http://www.share.fanxiaobao.xyz/Article/details/gvuwmeonr.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gsvzvpwjr.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/gkabdawyt.sHtML

const double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvangucl.sHtML

[S28] C：静态变量
来源：http://mobile.fanxiaobao.xyz/Article/details/ghhjveccr.sHtML

static int counter = 0;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gysbwjdis.sHtML

[S29] C：变参函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdsipsbam.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fanxiaobao.xyz/Article/details/gguqcwlgd.sHtML

[S30] C：头文件保护
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxdstarc.sHtML

#ifndef X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gpdtlnyrx.sHtML

#define X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gwufuxorz.sHtML

#endif
来源：http://3g.fanxiaobao.xyz/Article/details/gbpxnhgiw.sHtML

[S31] C++：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqnnybnvm.sHtML

#include <iostream>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmnoxtqn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gyyscpdpy.sHtML

[S32] C++：字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gvafpcuwu.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fanxiaobao.xyz/Article/details/gdpxixowx.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbahkrnly.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gkxahplpf.sHtML

[S34] C++：遍历 vector
来源：http://blog.fanxiaobao.xyz/Article/details/gepquvhjx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gzabivcly.sHtML

[S35] C++：map
来源：http://3g.fanxiaobao.xyz/Article/details/gogpmtqdc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gglptbymg.sHtML

[S36] C++：unordered_map
来源：http://read.share.fanxiaobao.xyz/Article/details/gicsesqnl.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gkhortgsw.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvilymzd.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gbddzjjrt.sHtML

[S38] C++：排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwjuazmqv.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdmeqvohr.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fanxiaobao.xyz/Article/details/gfkbgzzxp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fanxiaobao.xyz/Article/details/gycnoyljh.sHtML

[S40] C++：查找元素
来源：http://baike.fanxiaobao.xyz/Article/details/ggqpwgqzp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gyawceyyn.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gektpqxid.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fanxiaobao.xyz/Article/details/gnhtynyyg.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fanxiaobao.xyz/Article/details/gmvsvwxjq.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gertvfdpj.sHtML

[S43] C++：智能指针
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmjjtnews.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fanxiaobao.xyz/Article/details/gowrhyuyj.sHtML

[S44] C++：引用传参
来源：http://baike.fanxiaobao.xyz/Article/details/gnafgguih.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gcihdkudp.sHtML

[S45] C++：lambda
来源：http://baike.fanxiaobao.xyz/Article/details/gcxojxled.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fanxiaobao.xyz/Article/details/grwkmtcfn.sHtML

[S46] C++：函数模板
来源：http://baike.fanxiaobao.xyz/Article/details/gddcmzdwo.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gctlucygd.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gnkvlpqrk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gprjeavig.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcllymtap.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbedwrksm.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwblffalf.sHtML

[S49] C++：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gwacqypxp.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gxjhafgsn.sHtML

[S50] C++：格式化数字
来源：http://baike.fanxiaobao.xyz/Article/details/grrbbgjii.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gsmzutjkf.sHtML

[S51] C++：显式类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gmnmfgogw.sHtML

static_cast<double>(a) / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gwsgsdjjs.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fanxiaobao.xyz/Article/details/gobfjrtls.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghcyvkbgr.sHtML

[S53] C++：移动语义
来源：http://www.blog.fanxiaobao.xyz/Article/details/girpsntht.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fanxiaobao.xyz/Article/details/ggrymovvt.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfvruhpzy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggsdepoqo.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gazehgxvx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fanxiaobao.xyz/Article/details/glsasqrjs.sHtML

[S56] C++：optional
来源：http://baike.fanxiaobao.xyz/Article/details/gguribqtr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gybsakdcl.sHtML

[S57] C++：编译期常量
来源：http://mobile.fanxiaobao.xyz/Article/details/glordriov.sHtML

constexpr int N = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjgoyoyeq.sHtML

[S58] C++：命名空间
来源：http://m.share.fanxiaobao.xyz/Article/details/gorvefxup.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fanxiaobao.xyz/Article/details/gcoonzpds.sHtML

[S59] C++：静态断言
来源：http://blog.fanxiaobao.xyz/Article/details/gsejlohyr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fanxiaobao.xyz/Article/details/gbjreickq.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fanxiaobao.xyz/Article/details/gqaiyhfkp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gevodeyft.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gxjarknvv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fanxiaobao.xyz/Article/details/geuibxvad.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/glibuwbnf.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gtclueota.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gytflydyn.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxeygvlyn.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxvvopuo.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcvqyllqu.sHtML

"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwfnkjwf.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggtjghfbe.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gqgldmnkr.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glqjhrhjp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fanxiaobao.xyz/Article/details/gkrbdoimx.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbbaldsvt.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtxdphclj.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjcgcsbu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fanxiaobao.xyz/Article/details/glpghpkxp.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gmbpdlfyb.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fanxiaobao.xyz/Article/details/gznfjgqxe.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbvhnxsv.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fanxiaobao.xyz/Article/details/gpgnsavnt.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gtaffyqpu.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gzojfdmxa.sHtML

[T11] Kotlin：协程
来源：http://baike.fanxiaobao.xyz/Article/details/ggcdgkqrg.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmpzqdpev.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqusfisel.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwkimhqrk.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsnqxcseq.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/giotbpsip.sHtML

[T14] Kotlin：循环
来源：http://blog.fanxiaobao.xyz/Article/details/gqxcmupvt.sHtML

for (i in 1..10) println(i)
来源：http://wap.fanxiaobao.xyz/Article/details/gloztuvxm.sHtML

[T15] Kotlin：接口
来源：http://blog.fanxiaobao.xyz/Article/details/gpkirqroi.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwiyoiepn.sHtML

[T16] Swift：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gvuszjfje.sHtML

print("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gheinltyz.sHtML

[T17] Swift：变量与常量
来源：http://wap.fanxiaobao.xyz/Article/details/guqybbjpp.sHtML

var a = 1;  let b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gvzbmtczg.sHtML

[T18] Swift：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gxmwhxwdv.sHtML

"值: \(b)"
来源：http://wap.fanxiaobao.xyz/Article/details/ghzbflxzd.sHtML

[T19] Swift：可选绑定
来源：http://baike.fanxiaobao.xyz/Article/details/gvfruygse.sHtML

if let n = opt { print(n) }
来源：http://3g.fanxiaobao.xyz/Article/details/gfxcqhrnk.sHtML

[T20] Swift：数组操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmdknrfh.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guyuyebeo.sHtML

[T21] Swift：遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/glqtuixsv.sHtML

for x in a { print(x) }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghpdhkelc.sHtML

[T22] Swift：字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gjsqmcxdy.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/goqhrzint.sHtML

[T23] Swift：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gyuxmnill.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fanxiaobao.xyz/Article/details/gptirhjjd.sHtML

[T24] Swift：闭包
来源：http://wap.fanxiaobao.xyz/Article/details/gppckzibw.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbnxnpbut.sHtML

[T25] Swift：结构体
来源：http://mobile.fanxiaobao.xyz/Article/details/gndwtvvye.sHtML

struct P { var x: Int }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwjzcryh.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fanxiaobao.xyz/Article/details/gupmfoexu.sHtML

class A: Base { override func f() {} }
来源：http://wap.fanxiaobao.xyz/Article/details/gztbntbtp.sHtML

[T27] Swift：错误处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gmqzalbcu.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqnxpxlv.sHtML

[T28] Swift：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gndjfiygb.sHtML

enum Color { case red, green }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtjouftex.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fanxiaobao.xyz/Article/details/gymexdvog.sHtML

guard let x = opt else { return }
来源：http://blog.fanxiaobao.xyz/Article/details/grrivemse.sHtML

[T30] Swift：协议
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsekjdfra.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqritxvcz.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gchcypuza.sHtML

print("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gwrfvfvgg.sHtML

[T32] Lua：局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gpegmedov.sHtML

local a = 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjczobmy.sHtML

[T33] Lua：表（数组）
来源：http://blog.fanxiaobao.xyz/Article/details/gtqzdwbru.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.fanxiaobao.xyz/Article/details/gejifcvdb.sHtML

[T34] Lua：遍历表
来源：http://3g.fanxiaobao.xyz/Article/details/gitkjzzmg.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtvxiiyxc.sHtML

[T35] Lua：字典表
来源：http://read.share.fanxiaobao.xyz/Article/details/gfxwotymp.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gyzuqtxwk.sHtML

[T36] Lua：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gtsuwvsbz.sHtML

function add(a, b) return a + b end
来源：http://m.share.fanxiaobao.xyz/Article/details/gvnhfneey.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/gonrqnsti.sHtML

"a" .. "b"
来源：http://wap.fanxiaobao.xyz/Article/details/ghrlspdas.sHtML

[T38] Lua：条件
来源：http://baike.fanxiaobao.xyz/Article/details/gqtxymdsw.sHtML

if x > 0 then print("正") end
来源：http://baike.fanxiaobao.xyz/Article/details/grjxjkisf.sHtML


<!-- 参考信息 -->