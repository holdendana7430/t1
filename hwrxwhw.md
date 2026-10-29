代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://m.share.zdbjq.cn/Article/details/grerhcixr.sHtML

[R32] 参数个数校验
来源：http://www.m.share.hesvh.cn/Article/details/growgjait.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/gjzqnndmm.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fehbvm.com/Article/details/gvnqyoesl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.hesvh.cn/Article/details/gspbesyfq.sHtML

[R34] 退出时清理
来源：http://mobile.zdbjq.cn/Article/details/gncicfraz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/giurzoqly.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.hesvh.cn/Article/details/gjznfjpro.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.hesvh.cn/Article/details/gxntqgfuq.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.zdbjq.cn/Article/details/gbvwtrqgr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fehbvm.com/Article/details/gdqvmpwdn.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fehbvm.com/Article/details/gssovsgda.sHtML

files=$(ls -1)
来源：http://blog.hesvh.cn/Article/details/ggwbklfga.sHtML

[R38] 管道串联
来源：http://mobile.zdbjq.cn/Article/details/gyrzvckjw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.zdbjq.cn/Article/details/gtjidrgon.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.hesvh.cn/Article/details/gcrdovlbi.sHtML

cmd > out.log 2>&1
来源：http://blog.zdbjq.cn/Article/details/gobjmbtfw.sHtML

[R40] 追加写日志
来源：http://mobile.zdbjq.cn/Article/details/giebxwelf.sHtML

echo "log" >> out.log
来源：http://wap.zdbjq.cn/Article/details/gfhkmodza.sHtML

[R41] 丢弃输出
来源：http://www.share.zdbjq.cn/Article/details/gzmivjdei.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.hesvh.cn/Article/details/gbalvagzw.sHtML

[R42] 输入重定向
来源：http://wap.hesvh.cn/Article/details/gawkdfjte.sHtML

wc -l < a.txt
来源：http://m.share.zdbjq.cn/Article/details/gbhfqwdfk.sHtML

[R43] 按名字查找文件
来源：http://baike.fehbvm.com/Article/details/geeupfevq.sHtML

find . -name "*.log" -type f
来源：http://baike.zdbjq.cn/Article/details/gpzzuxnfi.sHtML

[R44] 按修改时间查找
来源：http://baike.hesvh.cn/Article/details/gstndcmbi.sHtML

find . -mtime -7 -type f
来源：http://blog.zdbjq.cn/Article/details/gpsublpvw.sHtML

[R45] 批量删除
来源：http://baike.hesvh.cn/Article/details/guolaktsw.sHtML

find . -name "*.tmp" -delete
来源：http://3g.zdbjq.cn/Article/details/gxtolxhaj.sHtML

[R46] 递归替换文件内容
来源：http://baike.zdbjq.cn/Article/details/guenccsvm.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fehbvm.com/Article/details/goukhvlgo.sHtML

[R47] sed 单行替换
来源：http://read.share.hesvh.cn/Article/details/guxlpmzpf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.zdbjq.cn/Article/details/grksmewsg.sHtML

[R48] awk 取指定列
来源：http://baike.hesvh.cn/Article/details/gotfdyzvi.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/guslssong.sHtML

[R49] awk 带条件
来源：http://baike.hesvh.cn/Article/details/gucsnkffx.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fehbvm.com/Article/details/gqzkuxkcc.sHtML

[R50] awk 求和
来源：http://www.share.zdbjq.cn/Article/details/grwwmgmrb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fehbvm.com/Article/details/guyyoxrhv.sHtML

[R51] 排序去重取前几
来源：http://baike.fehbvm.com/Article/details/gaxlaegqo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.zdbjq.cn/Article/details/gtqmzxywq.sHtML

[R52] 统计行数
来源：http://www.blog.hesvh.cn/Article/details/ginwbuszw.sHtML

wc -l a.txt
来源：http://3g.zdbjq.cn/Article/details/gvwvhwwop.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fehbvm.com/Article/details/gbspxvsoa.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fehbvm.com/Article/details/gspwgruud.sHtML

[R54] 比较两个文件
来源：http://3g.fehbvm.com/Article/details/gpckrdvsf.sHtML

diff a.txt b.txt
来源：http://read.share.zdbjq.cn/Article/details/gkpkhjfai.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fehbvm.com/Article/details/gvpjwehkj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fehbvm.com/Article/details/ggzcadpdu.sHtML

[R56] 远程拷贝
来源：http://baike.hesvh.cn/Article/details/glonlvujy.sHtML

scp file user@host:/path/
来源：http://www.share.hesvh.cn/Article/details/ggscvwcrh.sHtML

[R57] 远程执行命令
来源：http://www.blog.hesvh.cn/Article/details/gdldvbtqv.sHtML

ssh user@host 'uptime'
来源：http://baike.hesvh.cn/Article/details/grwgfupyq.sHtML

[R58] 下载文件
来源：http://3g.hesvh.cn/Article/details/gcwzmemfp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.zdbjq.cn/Article/details/gstsqesec.sHtML

[R59] 发 POST JSON
来源：http://mobile.fehbvm.com/Article/details/gmwjkhqik.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.hesvh.cn/Article/details/gbmrdgvej.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/gbjyeblxt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.hesvh.cn/Article/details/gckyaychd.sHtML

[R61] 磁盘占用
来源：http://3g.hesvh.cn/Article/details/gliqsvgjt.sHtML

df -h;  du -sh *
来源：http://m.share.zdbjq.cn/Article/details/gpmdgsnvh.sHtML

[R62] 找最占空间的文件
来源：http://mobile.zdbjq.cn/Article/details/giwzuisrl.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.hesvh.cn/Article/details/gneuycykb.sHtML

[R63] 内存与进程
来源：http://m.share.hesvh.cn/Article/details/gszgqkueq.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.zdbjq.cn/Article/details/gaqiggllh.sHtML

[R64] 结束进程
来源：http://read.share.fehbvm.com/Article/details/ghwihejyh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fehbvm.com/Article/details/gmpvrjdwy.sHtML

[R65] 查看端口占用
来源：http://wap.fehbvm.com/Article/details/gwpmuwdqd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.hesvh.cn/Article/details/giofdlpkg.sHtML

[R66] 定时任务
来源：http://www.blog.hesvh.cn/Article/details/gxripnlfg.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.zdbjq.cn/Article/details/gdolfrgoz.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fehbvm.com/Article/details/gfkgoibhw.sHtML

openssl rand -hex 16
来源：http://baike.hesvh.cn/Article/details/gwbvojkma.sHtML

[R68] 计算文件校验值
来源：http://m.share.hesvh.cn/Article/details/gnwxvjpkf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.hesvh.cn/Article/details/glsrfnmql.sHtML

[R69] 生成随机密码
来源：http://read.share.hesvh.cn/Article/details/grplqxtfh.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.zdbjq.cn/Article/details/gjkiryoct.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.hesvh.cn/Article/details/ggxyvookt.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fehbvm.com/Article/details/gptzpoazu.sHtML

[R71] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/gdevssurz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.zdbjq.cn/Article/details/gcfndjzji.sHtML

[R72] 等待端口就绪
来源：http://wap.zdbjq.cn/Article/details/gaexhajfx.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/gqfwfbvxs.sHtML

[R73] 分割大日志
来源：http://www.m.share.hesvh.cn/Article/details/gwghtjqoe.sHtML

split -l 1000 big.log part_
来源：http://www.share.fehbvm.com/Article/details/gglklirsd.sHtML

[R74] 批量重命名
来源：http://mobile.fehbvm.com/Article/details/gjkgfqspm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.zdbjq.cn/Article/details/grdzwgsbs.sHtML

[R75] 导出环境变量
来源：http://mobile.fehbvm.com/Article/details/gwjgswiqy.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.hesvh.cn/Article/details/gynrrbmgy.sHtML

[R76] 使用临时文件
来源：http://wap.fehbvm.com/Article/details/gdlbblvtz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gvdtkbcdr.sHtML

[R77] 读取用户输入
来源：http://read.share.hesvh.cn/Article/details/gxcmjqrga.sHtML

read -rp "请输入: " ans
来源：http://www.share.fehbvm.com/Article/details/gbtcqjzlu.sHtML

[R78] 交互式菜单
来源：http://wap.fehbvm.com/Article/details/gejngehlx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fehbvm.com/Article/details/gobwglvzx.sHtML

[R79] 解析命令行选项
来源：http://read.share.fehbvm.com/Article/details/gachzwzdi.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.hesvh.cn/Article/details/gjlypopij.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fehbvm.com/Article/details/grutmkoaw.sHtML

time ./run.sh
来源：http://read.share.hesvh.cn/Article/details/gzkcbsmli.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gpqegiecr.sHtML

S. C / C++ 专题
来源：http://www.blog.fehbvm.com/Article/details/godeaollw.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gsnmsmnye.sHtML

[S01] C：Hello World
来源：http://blog.zdbjq.cn/Article/details/gortqbkzw.sHtML

#include <stdio.h>
来源：http://blog.fehbvm.com/Article/details/gtzesrnqv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fehbvm.com/Article/details/grvtfkxth.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fehbvm.com/Article/details/guovobpuw.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fehbvm.com/Article/details/grfsodhie.sHtML

[S03] C：读入整数
来源：http://baike.zdbjq.cn/Article/details/guctqdnmc.sHtML

int x; scanf("%d", &x);
来源：http://wap.hesvh.cn/Article/details/gdkdoqgrm.sHtML

[S04] C：字符串复制
来源：http://www.share.fehbvm.com/Article/details/ggoabxymx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fehbvm.com/Article/details/gcjzeghua.sHtML

[S05] C：字符串长度
来源：http://mobile.fehbvm.com/Article/details/gwjekrdpq.sHtML

strlen(s)
来源：http://read.share.fehbvm.com/Article/details/gpjfrilkg.sHtML

[S06] C：字符串比较
来源：http://mobile.hesvh.cn/Article/details/ggwjrvgca.sHtML

strcmp(a, b) == 0
来源：http://wap.zdbjq.cn/Article/details/glegvwcvx.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.hesvh.cn/Article/details/gxolqlaqb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.zdbjq.cn/Article/details/gxwodmcye.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.hesvh.cn/Article/details/gwmfyrkzk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.zdbjq.cn/Article/details/gjnuegqrc.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.hesvh.cn/Article/details/giecbzotb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.hesvh.cn/Article/details/gyrpsvutr.sHtML

[S10] C：指针与解引用
来源：http://baike.fehbvm.com/Article/details/gdunevjhc.sHtML

int *p = &a;  *p = 5;
来源：http://3g.zdbjq.cn/Article/details/gpaflmmkv.sHtML

[S11] C：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/ggigsfnfy.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.hesvh.cn/Article/details/gwbnctvrm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.hesvh.cn/Article/details/gpdocrane.sHtML

fclose(f);
来源：http://3g.hesvh.cn/Article/details/gzxtpqauv.sHtML

[S12] C：写文件
来源：http://baike.hesvh.cn/Article/details/gefzfigia.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/ghosgbnrg.sHtML

[S13] C：宏定义
来源：http://3g.hesvh.cn/Article/details/gzzwsouvr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.zdbjq.cn/Article/details/gflblqbad.sHtML

[S14] C：枚举
来源：http://www.share.hesvh.cn/Article/details/gbsfjqwbe.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.zdbjq.cn/Article/details/ghdhtgtgo.sHtML

[S15] C：类型转换
来源：http://m.share.hesvh.cn/Article/details/gqpbfihmz.sHtML

(double) a / b
来源：http://baike.fehbvm.com/Article/details/gufajqfhv.sHtML

[S16] C：位操作置位
来源：http://www.share.hesvh.cn/Article/details/gweclheca.sHtML

x |= (1 << 3);
来源：http://3g.fehbvm.com/Article/details/grfsywoit.sHtML

[S17] C：安全拼接字符串
来源：http://3g.hesvh.cn/Article/details/gzubcoidz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.zdbjq.cn/Article/details/gigrvkxgo.sHtML

[S18] C：命令行参数
来源：http://www.share.hesvh.cn/Article/details/gsrpcwkeo.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.hesvh.cn/Article/details/gigflisob.sHtML

[S19] C：快速排序
来源：http://mobile.zdbjq.cn/Article/details/grvtnkket.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gatoaktpj.sHtML

[S20] C：二分查找
来源：http://baike.fehbvm.com/Article/details/gbubfephi.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/gxvfvymvo.sHtML

[S21] C：字符类别判断
来源：http://www.share.hesvh.cn/Article/details/grfidstls.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.hesvh.cn/Article/details/glrpihntf.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.hesvh.cn/Article/details/gxvggtziw.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.hesvh.cn/Article/details/gllhltwit.sHtML

[S23] C：随机数
来源：http://www.share.hesvh.cn/Article/details/gkyduosyj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.hesvh.cn/Article/details/gmrpsfvqd.sHtML

[S24] C：获取本地时间
来源：http://www.share.hesvh.cn/Article/details/glpdottbo.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fehbvm.com/Article/details/gpqzdquwk.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fehbvm.com/Article/details/gdydwbnla.sHtML

memcpy(dst, src, n);
来源：http://m.share.hesvh.cn/Article/details/gjoelnfah.sHtML

[S26] C：内存清零
来源：http://m.share.fehbvm.com/Article/details/gnkpayxza.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fehbvm.com/Article/details/geioaqbhm.sHtML

[S27] C：定义常量
来源：http://wap.zdbjq.cn/Article/details/glraupswj.sHtML

const double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gbgfnexuc.sHtML

[S28] C：静态变量
来源：http://wap.fehbvm.com/Article/details/gfgoquvoj.sHtML

static int counter = 0;
来源：http://read.share.hesvh.cn/Article/details/gitallaus.sHtML

[S29] C：变参函数
来源：http://mobile.zdbjq.cn/Article/details/gfkkrlads.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.zdbjq.cn/Article/details/ghrgytmqe.sHtML

[S30] C：头文件保护
来源：http://www.share.zdbjq.cn/Article/details/gtzzbgevy.sHtML

#ifndef X_H
来源：http://mobile.fehbvm.com/Article/details/gssfjguvo.sHtML

#define X_H
来源：http://wap.hesvh.cn/Article/details/ghfknkafc.sHtML

#endif
来源：http://blog.fehbvm.com/Article/details/gysgfuuxf.sHtML

[S31] C++：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gujcvfvay.sHtML

#include <iostream>
来源：http://read.share.zdbjq.cn/Article/details/ghywibkww.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.hesvh.cn/Article/details/gzomjzmdu.sHtML

[S32] C++：字符串
来源：http://m.share.fehbvm.com/Article/details/gpwnexvmd.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.zdbjq.cn/Article/details/gqataymea.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fehbvm.com/Article/details/goeijxqca.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.zdbjq.cn/Article/details/gwuixohod.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fehbvm.com/Article/details/gatfxubhc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.hesvh.cn/Article/details/gxhvkqara.sHtML

[S35] C++：map
来源：http://read.share.zdbjq.cn/Article/details/ghpelpfcp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gzfuyshni.sHtML

[S36] C++：unordered_map
来源：http://www.blog.hesvh.cn/Article/details/ghgjnpiwa.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/glzzdtusl.sHtML

[S37] C++：set
来源：http://www.share.hesvh.cn/Article/details/gcqhgyjiv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.hesvh.cn/Article/details/gyujdwlub.sHtML

[S38] C++：排序
来源：http://www.m.share.zdbjq.cn/Article/details/grmkqfllf.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.hesvh.cn/Article/details/gxgdmfipy.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.zdbjq.cn/Article/details/geztjmlsw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fehbvm.com/Article/details/ghdlgpdip.sHtML

[S40] C++：查找元素
来源：http://www.blog.zdbjq.cn/Article/details/gahpyhsqd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.zdbjq.cn/Article/details/gbytthgll.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.hesvh.cn/Article/details/gxbetdmcm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fehbvm.com/Article/details/gmmnjdiia.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.zdbjq.cn/Article/details/gszstmpls.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.zdbjq.cn/Article/details/glmscjacq.sHtML

[S43] C++：智能指针
来源：http://baike.hesvh.cn/Article/details/gmijqyjru.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.hesvh.cn/Article/details/gzaixqdbr.sHtML

[S44] C++：引用传参
来源：http://www.share.hesvh.cn/Article/details/gleaawfew.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fehbvm.com/Article/details/gfcnhqezb.sHtML

[S45] C++：lambda
来源：http://read.share.hesvh.cn/Article/details/gpcruouau.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fehbvm.com/Article/details/gvnuiamtw.sHtML

[S46] C++：函数模板
来源：http://www.share.zdbjq.cn/Article/details/gtvnziwoo.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.zdbjq.cn/Article/details/gyrrngech.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fehbvm.com/Article/details/gpxnohsbl.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.hesvh.cn/Article/details/gaibbrwda.sHtML

[S48] C++：逐行读文件
来源：http://baike.fehbvm.com/Article/details/ggahxviyx.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.zdbjq.cn/Article/details/gygshpjaz.sHtML

while (std::getline(in, line)) { }
来源：http://3g.zdbjq.cn/Article/details/glfoczgqo.sHtML

[S49] C++：写文件
来源：http://wap.hesvh.cn/Article/details/grahzgczz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.zdbjq.cn/Article/details/gpqpnhknv.sHtML

[S50] C++：格式化数字
来源：http://baike.zdbjq.cn/Article/details/gtjoxkjou.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.hesvh.cn/Article/details/gapwkeqlw.sHtML

[S51] C++：显式类型转换
来源：http://mobile.zdbjq.cn/Article/details/gbegnuogg.sHtML

static_cast<double>(a) / b
来源：http://blog.fehbvm.com/Article/details/gknhbpspx.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.hesvh.cn/Article/details/guawlhnxq.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fehbvm.com/Article/details/gufjtjfjp.sHtML

[S53] C++：移动语义
来源：http://baike.fehbvm.com/Article/details/gxjowmyiq.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.zdbjq.cn/Article/details/grfkevfme.sHtML

[S54] C++：异常处理
来源：http://blog.zdbjq.cn/Article/details/ghkuktytb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.hesvh.cn/Article/details/gqmebnrnv.sHtML

[S55] C++：结构化绑定
来源：http://blog.hesvh.cn/Article/details/goqydrszx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fehbvm.com/Article/details/ghrtiokuv.sHtML

[S56] C++：optional
来源：http://www.share.fehbvm.com/Article/details/ggglmzncx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.hesvh.cn/Article/details/gqprlbxdl.sHtML

[S57] C++：编译期常量
来源：http://read.share.hesvh.cn/Article/details/gcecaohxr.sHtML

constexpr int N = 10;
来源：http://wap.fehbvm.com/Article/details/gdyidepdt.sHtML

[S58] C++：命名空间
来源：http://www.m.share.hesvh.cn/Article/details/gxfjhvraj.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fehbvm.com/Article/details/grwqxmxiw.sHtML

[S59] C++：静态断言
来源：http://baike.hesvh.cn/Article/details/gyievkmgs.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.zdbjq.cn/Article/details/gklcaglaf.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.hesvh.cn/Article/details/gljlbghcy.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.hesvh.cn/Article/details/gjapydngr.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gozprhusn.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fehbvm.com/Article/details/gwitagupk.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/grlqjcilb.sHtML

[T01] Kotlin：Hello World
来源：http://wap.zdbjq.cn/Article/details/gntoqnlby.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/ghtrgxzbl.sHtML

[T02] Kotlin：变量
来源：http://3g.fehbvm.com/Article/details/ggcivmrar.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fehbvm.com/Article/details/glimsmrdh.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fehbvm.com/Article/details/gyhhxzona.sHtML

"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/guisevwgm.sHtML

[T04] Kotlin：空安全
来源：http://blog.hesvh.cn/Article/details/gyyujozgy.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fehbvm.com/Article/details/guytvvcoc.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.hesvh.cn/Article/details/glwpuafvc.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.hesvh.cn/Article/details/gnuridyrt.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fehbvm.com/Article/details/gceroyzyw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.hesvh.cn/Article/details/gnntfbezr.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fehbvm.com/Article/details/gndyanmdf.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fehbvm.com/Article/details/ghmlblmqx.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fehbvm.com/Article/details/gzvwektkj.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fehbvm.com/Article/details/gsbievabr.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.zdbjq.cn/Article/details/gnfwfrdkt.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.zdbjq.cn/Article/details/gvjfhbusz.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.hesvh.cn/Article/details/gohgbzpkg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fehbvm.com/Article/details/gxiqfgiqh.sHtML

[T11] Kotlin：协程
来源：http://m.share.fehbvm.com/Article/details/gwuvtypwf.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.hesvh.cn/Article/details/gpzxreqkd.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.zdbjq.cn/Article/details/gbqdvhinr.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.hesvh.cn/Article/details/gziasnwge.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.zdbjq.cn/Article/details/gleaxclhg.sHtML

val m = mapOf("a" to 1)
来源：http://blog.hesvh.cn/Article/details/gwfggcjlo.sHtML

[T14] Kotlin：循环
来源：http://read.share.fehbvm.com/Article/details/gdzqeaotd.sHtML

for (i in 1..10) println(i)
来源：http://3g.hesvh.cn/Article/details/gizuucgto.sHtML

[T15] Kotlin：接口
来源：http://wap.fehbvm.com/Article/details/gqviprrvb.sHtML

interface Shape { fun area(): Double }
来源：http://3g.zdbjq.cn/Article/details/geofwylbp.sHtML

[T16] Swift：Hello World
来源：http://read.share.fehbvm.com/Article/details/gzhrrpeqv.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/grmcqwbso.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fehbvm.com/Article/details/gxqcalnev.sHtML

var a = 1;  let b = 2
来源：http://3g.fehbvm.com/Article/details/geympydlz.sHtML

[T18] Swift：字符串插值
来源：http://baike.hesvh.cn/Article/details/gsitxzhik.sHtML

"值: \(b)"
来源：http://m.share.hesvh.cn/Article/details/gnxgybbji.sHtML

[T19] Swift：可选绑定
来源：http://mobile.zdbjq.cn/Article/details/gygetgtcz.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fehbvm.com/Article/details/gmdxjboyx.sHtML

[T20] Swift：数组操作
来源：http://www.share.fehbvm.com/Article/details/gpxxavgks.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fehbvm.com/Article/details/gbwmjrsbu.sHtML

[T21] Swift：遍历
来源：http://m.share.hesvh.cn/Article/details/gzwqqzecz.sHtML

for x in a { print(x) }
来源：http://www.blog.hesvh.cn/Article/details/gxetikrvc.sHtML

[T22] Swift：字典
来源：http://baike.zdbjq.cn/Article/details/gyrmbbjyi.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.zdbjq.cn/Article/details/gnbpktbru.sHtML

[T23] Swift：函数
来源：http://baike.hesvh.cn/Article/details/grrchqcpu.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.zdbjq.cn/Article/details/gsidhooei.sHtML

[T24] Swift：闭包
来源：http://mobile.zdbjq.cn/Article/details/grcimawfy.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gcpjuykhe.sHtML

[T25] Swift：结构体
来源：http://www.blog.zdbjq.cn/Article/details/gxqvmsdqu.sHtML

struct P { var x: Int }
来源：http://3g.hesvh.cn/Article/details/gmdikbogs.sHtML

[T26] Swift：类与重写
来源：http://3g.hesvh.cn/Article/details/gfcgemisk.sHtML

class A: Base { override func f() {} }
来源：http://baike.fehbvm.com/Article/details/ggjdypmcx.sHtML

[T27] Swift：错误处理
来源：http://blog.zdbjq.cn/Article/details/gawkwqezg.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.zdbjq.cn/Article/details/gwnebdotd.sHtML

[T28] Swift：枚举
来源：http://baike.hesvh.cn/Article/details/gpzrqbnuo.sHtML

enum Color { case red, green }
来源：http://www.blog.hesvh.cn/Article/details/gfdmngpio.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fehbvm.com/Article/details/gmcdgzyek.sHtML

guard let x = opt else { return }
来源：http://3g.hesvh.cn/Article/details/gnuopjsio.sHtML

[T30] Swift：协议
来源：http://blog.fehbvm.com/Article/details/gathwhssx.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.zdbjq.cn/Article/details/gtxfhyypa.sHtML

[T31] Lua：Hello World
来源：http://wap.hesvh.cn/Article/details/grpqrihrl.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/grdxcnmdc.sHtML

[T32] Lua：局部变量
来源：http://mobile.zdbjq.cn/Article/details/gsaixtsxn.sHtML

local a = 1
来源：http://www.blog.zdbjq.cn/Article/details/gyxfsnmrj.sHtML

[T33] Lua：表（数组）
来源：http://blog.zdbjq.cn/Article/details/gzrwrzgei.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.hesvh.cn/Article/details/gsiiknzch.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.zdbjq.cn/Article/details/grsuvqhgo.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.hesvh.cn/Article/details/gjbcqijgw.sHtML


<!-- 参考信息 -->