代发 wailian999

echo $((1 + 2 * 3))
来源：http://wap.zdbjq.cn/Article/details/gqdwjvjsa.sHtML

[R28] 浮点运算
来源：http://www.m.share.hesvh.cn/Article/details/gsixjbmqu.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.hesvh.cn/Article/details/gssxmkixt.sHtML

[R29] 定义函数
来源：http://3g.fehbvm.com/Article/details/gulatilyf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fehbvm.com/Article/details/gxgejfkud.sHtML

[R30] 函数返回状态码
来源：http://wap.hesvh.cn/Article/details/gwyfezgxo.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.hesvh.cn/Article/details/gwhzzydfh.sHtML

[R31] 局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gqlrcgpxa.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fehbvm.com/Article/details/gfrmtfckl.sHtML

[R32] 参数个数校验
来源：http://www.blog.hesvh.cn/Article/details/gaodjwhyl.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/gslxmxzcb.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fehbvm.com/Article/details/gaitkudwp.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.zdbjq.cn/Article/details/gtbkohpau.sHtML

[R34] 退出时清理
来源：http://read.share.hesvh.cn/Article/details/glmjqylyx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/gytqxdsuz.sHtML

[R35] 后台执行并等待
来源：http://mobile.fehbvm.com/Article/details/gcssxywuc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.hesvh.cn/Article/details/gvbjriicr.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.hesvh.cn/Article/details/gqdayfgle.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.hesvh.cn/Article/details/glclgoaqm.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.hesvh.cn/Article/details/gjkuhjwel.sHtML

files=$(ls -1)
来源：http://wap.fehbvm.com/Article/details/gryagvonp.sHtML

[R38] 管道串联
来源：http://m.share.fehbvm.com/Article/details/guzjmzxez.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.zdbjq.cn/Article/details/glcuphjze.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.zdbjq.cn/Article/details/gfgnndpvx.sHtML

cmd > out.log 2>&1
来源：http://mobile.zdbjq.cn/Article/details/gcetoixjl.sHtML

[R40] 追加写日志
来源：http://blog.zdbjq.cn/Article/details/gcqenzqqw.sHtML

echo "log" >> out.log
来源：http://baike.fehbvm.com/Article/details/gdaiprtgq.sHtML

[R41] 丢弃输出
来源：http://read.share.hesvh.cn/Article/details/gqafufrhp.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.hesvh.cn/Article/details/gcgseegxu.sHtML

[R42] 输入重定向
来源：http://3g.hesvh.cn/Article/details/gopxocrjt.sHtML

wc -l < a.txt
来源：http://mobile.hesvh.cn/Article/details/gukzmvfpq.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.hesvh.cn/Article/details/gzrgfxsqj.sHtML

find . -name "*.log" -type f
来源：http://mobile.fehbvm.com/Article/details/gxcvrjghm.sHtML

[R44] 按修改时间查找
来源：http://mobile.hesvh.cn/Article/details/gugbzfrzj.sHtML

find . -mtime -7 -type f
来源：http://mobile.fehbvm.com/Article/details/gsiixgghd.sHtML

[R45] 批量删除
来源：http://3g.zdbjq.cn/Article/details/glzqqrtkm.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.zdbjq.cn/Article/details/gxuryuyml.sHtML

[R46] 递归替换文件内容
来源：http://www.share.zdbjq.cn/Article/details/gqyiujkrg.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.zdbjq.cn/Article/details/gjntkliku.sHtML

[R47] sed 单行替换
来源：http://read.share.zdbjq.cn/Article/details/gljkzwdok.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.hesvh.cn/Article/details/gewnhbhwm.sHtML

[R48] awk 取指定列
来源：http://www.share.fehbvm.com/Article/details/gklnzdfze.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.hesvh.cn/Article/details/gdekhsmum.sHtML

[R49] awk 带条件
来源：http://www.m.share.zdbjq.cn/Article/details/gapkwiovi.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.zdbjq.cn/Article/details/gyhlwlkct.sHtML

[R50] awk 求和
来源：http://www.m.share.fehbvm.com/Article/details/gujwpplav.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.hesvh.cn/Article/details/gfrxgijkz.sHtML

[R51] 排序去重取前几
来源：http://blog.zdbjq.cn/Article/details/gaykohgmh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.zdbjq.cn/Article/details/gomghecgt.sHtML

[R52] 统计行数
来源：http://read.share.hesvh.cn/Article/details/gicpcxtkf.sHtML

wc -l a.txt
来源：http://m.share.zdbjq.cn/Article/details/ghmeljuhr.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fehbvm.com/Article/details/gmyeqjezh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fehbvm.com/Article/details/gwqjjuqxr.sHtML

[R54] 比较两个文件
来源：http://www.blog.zdbjq.cn/Article/details/gwqagsxjh.sHtML

diff a.txt b.txt
来源：http://mobile.fehbvm.com/Article/details/gtdmzfvzl.sHtML

[R55] 压缩与解压
来源：http://wap.fehbvm.com/Article/details/goltzngug.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.hesvh.cn/Article/details/gikwbbjpq.sHtML

[R56] 远程拷贝
来源：http://3g.zdbjq.cn/Article/details/gfnfwgtyv.sHtML

scp file user@host:/path/
来源：http://3g.zdbjq.cn/Article/details/grmwhhoge.sHtML

[R57] 远程执行命令
来源：http://3g.fehbvm.com/Article/details/gwomasotx.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.zdbjq.cn/Article/details/gjweksvgm.sHtML

[R58] 下载文件
来源：http://www.blog.hesvh.cn/Article/details/gadrlkivr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fehbvm.com/Article/details/gjolnxugs.sHtML

[R59] 发 POST JSON
来源：http://baike.fehbvm.com/Article/details/gibsmfnoo.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.zdbjq.cn/Article/details/gpfdzvwzw.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/ghmrjtxlp.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.zdbjq.cn/Article/details/gbaefngqq.sHtML

[R61] 磁盘占用
来源：http://baike.zdbjq.cn/Article/details/gzcpjlqcz.sHtML

df -h;  du -sh *
来源：http://m.share.fehbvm.com/Article/details/gmilwzksn.sHtML

[R62] 找最占空间的文件
来源：http://wap.fehbvm.com/Article/details/grkjltdes.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fehbvm.com/Article/details/gjhwziyxi.sHtML

[R63] 内存与进程
来源：http://baike.fehbvm.com/Article/details/gmqoomtcl.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.zdbjq.cn/Article/details/gfvykacuq.sHtML

[R64] 结束进程
来源：http://www.share.hesvh.cn/Article/details/guuoofkgs.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fehbvm.com/Article/details/glmohfhhe.sHtML

[R65] 查看端口占用
来源：http://www.share.hesvh.cn/Article/details/glmmdomme.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fehbvm.com/Article/details/gymskjiau.sHtML

[R66] 定时任务
来源：http://www.m.share.hesvh.cn/Article/details/gqjooakbl.sHtML

crontab -e;  crontab -l
来源：http://wap.zdbjq.cn/Article/details/gnavrhejo.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fehbvm.com/Article/details/gvihtpqca.sHtML

openssl rand -hex 16
来源：http://wap.zdbjq.cn/Article/details/gapqkebks.sHtML

[R68] 计算文件校验值
来源：http://wap.fehbvm.com/Article/details/gpfkpusvz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.hesvh.cn/Article/details/gwzhyqrru.sHtML

[R69] 生成随机密码
来源：http://blog.zdbjq.cn/Article/details/gomedfwbl.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.zdbjq.cn/Article/details/gmpzwxisk.sHtML

[R70] 时间戳与互转
来源：http://mobile.hesvh.cn/Article/details/gqamquhxo.sHtML

date +%s;  date -d @1700000000
来源：http://baike.zdbjq.cn/Article/details/gvfdmhcde.sHtML

[R71] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gvprrklct.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fehbvm.com/Article/details/gfdyxkzol.sHtML

[R72] 等待端口就绪
来源：http://www.share.hesvh.cn/Article/details/gihbnibuf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gfvvgqnml.sHtML

[R73] 分割大日志
来源：http://baike.fehbvm.com/Article/details/grzegeshj.sHtML

split -l 1000 big.log part_
来源：http://www.blog.hesvh.cn/Article/details/gtkvuezlt.sHtML

[R74] 批量重命名
来源：http://www.m.share.hesvh.cn/Article/details/gwnzqlvfh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.zdbjq.cn/Article/details/gnbgyxwqr.sHtML

[R75] 导出环境变量
来源：http://wap.zdbjq.cn/Article/details/gaiahnjmw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.hesvh.cn/Article/details/gylycpqgn.sHtML

[R76] 使用临时文件
来源：http://www.m.share.zdbjq.cn/Article/details/gqijxaidh.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/gtwshnydu.sHtML

[R77] 读取用户输入
来源：http://wap.hesvh.cn/Article/details/gamksttiv.sHtML

read -rp "请输入: " ans
来源：http://wap.fehbvm.com/Article/details/gkdtyvfaz.sHtML

[R78] 交互式菜单
来源：http://mobile.zdbjq.cn/Article/details/gykchzaui.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.zdbjq.cn/Article/details/gaubuzrfz.sHtML

[R79] 解析命令行选项
来源：http://wap.hesvh.cn/Article/details/gtzasrefr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.hesvh.cn/Article/details/grahemgcx.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.hesvh.cn/Article/details/gnhcufull.sHtML

time ./run.sh
来源：http://baike.zdbjq.cn/Article/details/gggeycvry.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gtzmwfpxq.sHtML

S. C / C++ 专题
来源：http://m.share.zdbjq.cn/Article/details/gnhzvbvnb.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/guzaqxyqd.sHtML

[S01] C：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gtowznxfj.sHtML

#include <stdio.h>
来源：http://www.share.hesvh.cn/Article/details/gqdwmatnp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fehbvm.com/Article/details/gjnmlqkbp.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fehbvm.com/Article/details/ghsxcqpee.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.hesvh.cn/Article/details/ghaskrzsz.sHtML

[S03] C：读入整数
来源：http://mobile.zdbjq.cn/Article/details/gyauwzhfc.sHtML

int x; scanf("%d", &x);
来源：http://3g.hesvh.cn/Article/details/gnwyfjqdb.sHtML

[S04] C：字符串复制
来源：http://read.share.hesvh.cn/Article/details/gskaplttl.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fehbvm.com/Article/details/gfuapxwbw.sHtML

[S05] C：字符串长度
来源：http://blog.hesvh.cn/Article/details/gxcnmyzpb.sHtML

strlen(s)
来源：http://blog.zdbjq.cn/Article/details/gsmjirsdc.sHtML

[S06] C：字符串比较
来源：http://m.share.zdbjq.cn/Article/details/gxpcbqbgq.sHtML

strcmp(a, b) == 0
来源：http://3g.hesvh.cn/Article/details/gzphkagfh.sHtML

[S07] C：数组遍历求和
来源：http://wap.hesvh.cn/Article/details/gfemobvip.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.hesvh.cn/Article/details/gxfsoybbm.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fehbvm.com/Article/details/gboqrqgux.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.zdbjq.cn/Article/details/gfitiglio.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.zdbjq.cn/Article/details/gulzkofab.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.hesvh.cn/Article/details/gszzajfha.sHtML

[S10] C：指针与解引用
来源：http://mobile.zdbjq.cn/Article/details/gdfxzpoga.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.zdbjq.cn/Article/details/gexvvhsck.sHtML

[S11] C：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gybjxfvtw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.hesvh.cn/Article/details/gqobmwrgh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.zdbjq.cn/Article/details/gwdsywxqw.sHtML

fclose(f);
来源：http://m.share.fehbvm.com/Article/details/gozppahif.sHtML

[S12] C：写文件
来源：http://3g.fehbvm.com/Article/details/gtnmaejja.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.hesvh.cn/Article/details/glvgiwfpk.sHtML

[S13] C：宏定义
来源：http://www.blog.hesvh.cn/Article/details/gwwomoreg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fehbvm.com/Article/details/gorsicjcm.sHtML

[S14] C：枚举
来源：http://www.blog.zdbjq.cn/Article/details/gbmxourhp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.hesvh.cn/Article/details/gdqcreofw.sHtML

[S15] C：类型转换
来源：http://blog.zdbjq.cn/Article/details/gbgxzlbsy.sHtML

(double) a / b
来源：http://mobile.zdbjq.cn/Article/details/gcqujvvxg.sHtML

[S16] C：位操作置位
来源：http://blog.fehbvm.com/Article/details/gqstjvdkv.sHtML

x |= (1 << 3);
来源：http://www.share.zdbjq.cn/Article/details/gijyuuulg.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fehbvm.com/Article/details/ggiyglhmj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.zdbjq.cn/Article/details/gbqjzjnuj.sHtML

[S18] C：命令行参数
来源：http://blog.fehbvm.com/Article/details/gtekoyhkq.sHtML

int main(int argc, char **argv)
来源：http://baike.zdbjq.cn/Article/details/gqnosrids.sHtML

[S19] C：快速排序
来源：http://read.share.fehbvm.com/Article/details/gjyasnjfy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gtxfboyvc.sHtML

[S20] C：二分查找
来源：http://blog.fehbvm.com/Article/details/grfjagnbp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gzsiqgnle.sHtML

[S21] C：字符类别判断
来源：http://wap.fehbvm.com/Article/details/gmwqcssog.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.hesvh.cn/Article/details/grumsrkjy.sHtML

[S22] C：字符串转数字
来源：http://blog.zdbjq.cn/Article/details/gjezghdrg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.hesvh.cn/Article/details/gcnofqmdz.sHtML

[S23] C：随机数
来源：http://www.share.zdbjq.cn/Article/details/glhetdotd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fehbvm.com/Article/details/gednraxyy.sHtML

[S24] C：获取本地时间
来源：http://mobile.hesvh.cn/Article/details/gitzabxlx.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.zdbjq.cn/Article/details/ghsbfpvjr.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gwhofljdj.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fehbvm.com/Article/details/gdpzpuaeo.sHtML

[S26] C：内存清零
来源：http://www.m.share.hesvh.cn/Article/details/gtjgabovn.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fehbvm.com/Article/details/givddkanj.sHtML

[S27] C：定义常量
来源：http://www.blog.zdbjq.cn/Article/details/ggjnxbtvp.sHtML

const double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gcxukavpe.sHtML

[S28] C：静态变量
来源：http://m.share.fehbvm.com/Article/details/gzunivumb.sHtML

static int counter = 0;
来源：http://baike.fehbvm.com/Article/details/gednsrmll.sHtML

[S29] C：变参函数
来源：http://wap.zdbjq.cn/Article/details/gxatpzmnd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.hesvh.cn/Article/details/gygzjxaas.sHtML

[S30] C：头文件保护
来源：http://wap.zdbjq.cn/Article/details/gxoplsfyf.sHtML

#ifndef X_H
来源：http://blog.fehbvm.com/Article/details/gylwpuedh.sHtML

#define X_H
来源：http://baike.fehbvm.com/Article/details/gxnjidjsc.sHtML

#endif
来源：http://baike.zdbjq.cn/Article/details/getluwycj.sHtML

[S31] C++：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gndphazxl.sHtML

#include <iostream>
来源：http://read.share.fehbvm.com/Article/details/gkrkqmqfl.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.zdbjq.cn/Article/details/gwwhtjmme.sHtML

[S32] C++：字符串
来源：http://www.blog.hesvh.cn/Article/details/gsttazecs.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.zdbjq.cn/Article/details/gwlicbliu.sHtML

[S33] C++：vector 增删
来源：http://m.share.zdbjq.cn/Article/details/gkuunnhhc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.zdbjq.cn/Article/details/gbsbrcakq.sHtML

[S34] C++：遍历 vector
来源：http://mobile.zdbjq.cn/Article/details/gdppascqf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.zdbjq.cn/Article/details/guzigsiat.sHtML

[S35] C++：map
来源：http://mobile.fehbvm.com/Article/details/gtsrdqaum.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gomvuofcf.sHtML

[S36] C++：unordered_map
来源：http://m.share.zdbjq.cn/Article/details/gpoectuji.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fehbvm.com/Article/details/grshwpque.sHtML

[S37] C++：set
来源：http://wap.hesvh.cn/Article/details/glaydlhkh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.zdbjq.cn/Article/details/gwjotnalm.sHtML

[S38] C++：排序
来源：http://www.blog.fehbvm.com/Article/details/ghhakuqbt.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.hesvh.cn/Article/details/gbxvorebe.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.hesvh.cn/Article/details/gvnbfqvdm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fehbvm.com/Article/details/gvcftwygc.sHtML

[S40] C++：查找元素
来源：http://www.share.hesvh.cn/Article/details/giarfdqgg.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gjzgbeadj.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gcwmgcyky.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fehbvm.com/Article/details/gkytvxuqw.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fehbvm.com/Article/details/gezdwtrej.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.hesvh.cn/Article/details/ghmdueqar.sHtML

[S43] C++：智能指针
来源：http://m.share.zdbjq.cn/Article/details/gdeoylowx.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.zdbjq.cn/Article/details/gajkivsui.sHtML

[S44] C++：引用传参
来源：http://baike.zdbjq.cn/Article/details/gfhvlutra.sHtML

void inc(int &x) { ++x; }
来源：http://wap.zdbjq.cn/Article/details/guzfyfmqo.sHtML

[S45] C++：lambda
来源：http://www.m.share.hesvh.cn/Article/details/glppolwnq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.zdbjq.cn/Article/details/glkxdxkyg.sHtML

[S46] C++：函数模板
来源：http://www.m.share.hesvh.cn/Article/details/gxvpvhwxy.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.hesvh.cn/Article/details/giauyksjk.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.zdbjq.cn/Article/details/gxoaajtzy.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.zdbjq.cn/Article/details/gbecktlgr.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gozygawiv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fehbvm.com/Article/details/gydguzscu.sHtML

while (std::getline(in, line)) { }
来源：http://blog.hesvh.cn/Article/details/gdfqrialn.sHtML

[S49] C++：写文件
来源：http://www.m.share.fehbvm.com/Article/details/grcveuazs.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.hesvh.cn/Article/details/gfqgswmga.sHtML

[S50] C++：格式化数字
来源：http://mobile.hesvh.cn/Article/details/gugvicoyh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fehbvm.com/Article/details/gfzvdofhh.sHtML

[S51] C++：显式类型转换
来源：http://wap.zdbjq.cn/Article/details/gngfsnfvl.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fehbvm.com/Article/details/gqzsekwat.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.zdbjq.cn/Article/details/geztkpjez.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fehbvm.com/Article/details/gljczoaxm.sHtML

[S53] C++：移动语义
来源：http://www.blog.hesvh.cn/Article/details/gbzizyeqm.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.zdbjq.cn/Article/details/ghwaqrquq.sHtML

[S54] C++：异常处理
来源：http://blog.hesvh.cn/Article/details/gtkikpnyq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.zdbjq.cn/Article/details/gyyutclby.sHtML

[S55] C++：结构化绑定
来源：http://blog.hesvh.cn/Article/details/gnfhkuxva.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.zdbjq.cn/Article/details/gswsbydkd.sHtML

[S56] C++：optional
来源：http://baike.zdbjq.cn/Article/details/gfvwjikuj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.zdbjq.cn/Article/details/gbxufmqlr.sHtML

[S57] C++：编译期常量
来源：http://mobile.hesvh.cn/Article/details/giurfcboi.sHtML

constexpr int N = 10;
来源：http://blog.fehbvm.com/Article/details/gcnpucyak.sHtML

[S58] C++：命名空间
来源：http://www.blog.zdbjq.cn/Article/details/gazkuqmer.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.hesvh.cn/Article/details/gyfxaanmv.sHtML

[S59] C++：静态断言
来源：http://baike.zdbjq.cn/Article/details/gcairhgbb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.hesvh.cn/Article/details/gvvfwmleb.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fehbvm.com/Article/details/gfebrybpe.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.hesvh.cn/Article/details/gfbgugtxu.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gusclgtis.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.zdbjq.cn/Article/details/gukivaujp.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gfoqjgflx.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fehbvm.com/Article/details/gktlfpkvg.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gwxywlrvn.sHtML

[T02] Kotlin：变量
来源：http://m.share.fehbvm.com/Article/details/gfwpzvsfw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.hesvh.cn/Article/details/gjencenjo.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fehbvm.com/Article/details/gdwhjlttb.sHtML

"值: $b"
来源：http://mobile.fehbvm.com/Article/details/gviisryhy.sHtML

[T04] Kotlin：空安全
来源：http://baike.fehbvm.com/Article/details/gadzqysii.sHtML

val n: String? = null;  n?.length
来源：http://wap.fehbvm.com/Article/details/ggvkxhdra.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.zdbjq.cn/Article/details/golwgfooh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.zdbjq.cn/Article/details/gbexlmgoi.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fehbvm.com/Article/details/gumfxyapu.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.zdbjq.cn/Article/details/gousiigyk.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.zdbjq.cn/Article/details/gotrpxkpv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.hesvh.cn/Article/details/gfeudvxhv.sHtML

[T08] Kotlin：数据类
来源：http://3g.zdbjq.cn/Article/details/gahohnfzd.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fehbvm.com/Article/details/gxftvseeb.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.hesvh.cn/Article/details/gcpmtfqcb.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.zdbjq.cn/Article/details/gaaxpjrfx.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fehbvm.com/Article/details/gdflmuuko.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.hesvh.cn/Article/details/gjugrnwms.sHtML

[T11] Kotlin：协程
来源：http://blog.hesvh.cn/Article/details/gvgzjdwea.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.hesvh.cn/Article/details/gechxdutw.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fehbvm.com/Article/details/gtomtfqbz.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gdvqdsbin.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.hesvh.cn/Article/details/giimqdquo.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fehbvm.com/Article/details/gdeedasrw.sHtML

[T14] Kotlin：循环
来源：http://read.share.fehbvm.com/Article/details/gzurqqyug.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fehbvm.com/Article/details/gmtlalelc.sHtML

[T15] Kotlin：接口
来源：http://baike.zdbjq.cn/Article/details/golvwaort.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.hesvh.cn/Article/details/gghmgsmgp.sHtML

[T16] Swift：Hello World
来源：http://www.share.hesvh.cn/Article/details/godnsdeax.sHtML

print("Hello")
来源：http://wap.hesvh.cn/Article/details/gtvpnesel.sHtML

[T17] Swift：变量与常量
来源：http://mobile.zdbjq.cn/Article/details/gbuipfeeb.sHtML

var a = 1;  let b = 2
来源：http://baike.fehbvm.com/Article/details/glrqowgom.sHtML

[T18] Swift：字符串插值
来源：http://baike.fehbvm.com/Article/details/glhzzhqxq.sHtML

"值: \(b)"
来源：http://baike.zdbjq.cn/Article/details/ghaaoiiem.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.zdbjq.cn/Article/details/gwtsrvcwo.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.zdbjq.cn/Article/details/ghgsubuzj.sHtML

[T20] Swift：数组操作
来源：http://wap.zdbjq.cn/Article/details/gndhpjwoi.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.hesvh.cn/Article/details/gabigtsqu.sHtML

[T21] Swift：遍历
来源：http://mobile.zdbjq.cn/Article/details/gckfjwgii.sHtML

for x in a { print(x) }
来源：http://www.blog.zdbjq.cn/Article/details/gcbygwqir.sHtML

[T22] Swift：字典
来源：http://www.blog.zdbjq.cn/Article/details/gbrthvvfq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.hesvh.cn/Article/details/gbolgmsxm.sHtML

[T23] Swift：函数
来源：http://wap.fehbvm.com/Article/details/ggaqoisbh.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.hesvh.cn/Article/details/gvvlfhbap.sHtML

[T24] Swift：闭包
来源：http://www.share.hesvh.cn/Article/details/gkzyxswvl.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gfzsktbgh.sHtML

[T25] Swift：结构体
来源：http://blog.zdbjq.cn/Article/details/gykngymad.sHtML

struct P { var x: Int }
来源：http://read.share.fehbvm.com/Article/details/gmvmmcjdb.sHtML

[T26] Swift：类与重写
来源：http://wap.hesvh.cn/Article/details/gyuuutfrb.sHtML

class A: Base { override func f() {} }
来源：http://wap.hesvh.cn/Article/details/gflmhdwgi.sHtML

[T27] Swift：错误处理
来源：http://m.share.hesvh.cn/Article/details/grawomxhr.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.zdbjq.cn/Article/details/ggxtjtrgg.sHtML

[T28] Swift：枚举
来源：http://wap.hesvh.cn/Article/details/gyjvndubo.sHtML

enum Color { case red, green }
来源：http://m.share.hesvh.cn/Article/details/gxveguzcy.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fehbvm.com/Article/details/gcddaitmw.sHtML

guard let x = opt else { return }
来源：http://mobile.zdbjq.cn/Article/details/ggefbtdcf.sHtML

[T30] Swift：协议
来源：http://www.share.fehbvm.com/Article/details/gdxkdfief.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.zdbjq.cn/Article/details/gtmamlfcp.sHtML


<!-- 参考信息 -->