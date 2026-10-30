代发 wailian999

echo "${#arr[@]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlrahwqk.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjamkewp.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gsgbsexws.sHtML

[R21] 字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/giuyadvbu.sHtML

echo "${#s}"
来源：http://baike.fanxiaobao.xyz/Article/details/gvorlwoqa.sHtML

[R22] 截取子串
来源：http://m.share.fanxiaobao.xyz/Article/details/gycuqthul.sHtML

echo "${s:0:5}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmedcpou.sHtML

[R23] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwiejipt.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fanxiaobao.xyz/Article/details/gkujotwla.sHtML

[R24] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gxjqbvuxv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fanxiaobao.xyz/Article/details/ggghjswrr.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fanxiaobao.xyz/Article/details/geouxmvme.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gewlgjgbw.sHtML

[R26] 命令替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjqjwtrq.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gllrvggjt.sHtML

[R27] 算术展开
来源：http://m.share.fanxiaobao.xyz/Article/details/gdgegfbye.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fanxiaobao.xyz/Article/details/gshblbzkj.sHtML

[R28] 浮点运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggdcpdqzt.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fanxiaobao.xyz/Article/details/guklzyhzc.sHtML

[R29] 定义函数
来源：http://wap.fanxiaobao.xyz/Article/details/gqeudfrdd.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsrxctuiu.sHtML

[R30] 函数返回状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gpihvojlm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fanxiaobao.xyz/Article/details/gehtiatgx.sHtML

[R31] 局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gomjsooph.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gfkhxqzvr.sHtML

[R32] 参数个数校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gvofepube.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggatnuvsb.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gipkzfeql.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/gbxxnainm.sHtML

[R34] 退出时清理
来源：http://www.share.fanxiaobao.xyz/Article/details/gfmnxsecl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gxvstsiqe.sHtML

[R35] 后台执行并等待
来源：http://blog.fanxiaobao.xyz/Article/details/gphzsiggq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fanxiaobao.xyz/Article/details/grouobyyo.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gjixxrvus.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fanxiaobao.xyz/Article/details/gzfeuzsse.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gdmvuuvng.sHtML

files=$(ls -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaqvwvohk.sHtML

[R38] 管道串联
来源：http://baike.fanxiaobao.xyz/Article/details/gkjljdzmj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbhwwuwf.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fanxiaobao.xyz/Article/details/ggxdhhktl.sHtML

cmd > out.log 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gwdgcetyq.sHtML

[R40] 追加写日志
来源：http://baike.fanxiaobao.xyz/Article/details/ghypcdzqy.sHtML

echo "log" >> out.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gumslemoe.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzeaaxutz.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gduuhwwoa.sHtML

[R42] 输入重定向
来源：http://mobile.fanxiaobao.xyz/Article/details/gjwiprrcc.sHtML

wc -l < a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gazzrgtma.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdobieueb.sHtML

find . -name "*.log" -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gfhjmmxbn.sHtML

[R44] 按修改时间查找
来源：http://blog.fanxiaobao.xyz/Article/details/gsqaycifk.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/giuuhvwgp.sHtML

[R45] 批量删除
来源：http://baike.fanxiaobao.xyz/Article/details/gmvtzopjp.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjigaxbsk.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fanxiaobao.xyz/Article/details/gblidchax.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fanxiaobao.xyz/Article/details/gotbsxems.sHtML

[R47] sed 单行替换
来源：http://blog.fanxiaobao.xyz/Article/details/gfaskgyvy.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gpybcdmsf.sHtML

[R48] awk 取指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/gmqiqttpn.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gflgdltax.sHtML

[R49] awk 带条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gnyekbwkh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fanxiaobao.xyz/Article/details/gfhutfnup.sHtML

[R50] awk 求和
来源：http://3g.fanxiaobao.xyz/Article/details/gtwggapxa.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtgpoalun.sHtML

[R51] 排序去重取前几
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxifvznr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fanxiaobao.xyz/Article/details/gighhihak.sHtML

[R52] 统计行数
来源：http://mobile.fanxiaobao.xyz/Article/details/goandhrox.sHtML

wc -l a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gaznwfjjd.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fanxiaobao.xyz/Article/details/gobswdkdc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fanxiaobao.xyz/Article/details/gckebmqvf.sHtML

[R54] 比较两个文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gsdzystyy.sHtML

diff a.txt b.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gonpbbfov.sHtML

[R55] 压缩与解压
来源：http://3g.fanxiaobao.xyz/Article/details/gfftdhlib.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzbogvwup.sHtML

[R56] 远程拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gmaumzfqj.sHtML

scp file user@host:/path/
来源：http://www.blog.fanxiaobao.xyz/Article/details/glhbhfput.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/gipxgihkk.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbtksaewb.sHtML

[R58] 下载文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvtavblgk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fanxiaobao.xyz/Article/details/gqwpzlzlb.sHtML

[R59] 发 POST JSON
来源：http://3g.fanxiaobao.xyz/Article/details/ghtvuleea.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fanxiaobao.xyz/Article/details/gifbjqtzo.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gypgrrxai.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fanxiaobao.xyz/Article/details/gfnhgtuep.sHtML

[R61] 磁盘占用
来源：http://www.share.fanxiaobao.xyz/Article/details/genopkhqf.sHtML

df -h;  du -sh *
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmqihdrwk.sHtML

[R62] 找最占空间的文件
来源：http://baike.fanxiaobao.xyz/Article/details/gwvgmlzii.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fanxiaobao.xyz/Article/details/gwjvafemx.sHtML

[R63] 内存与进程
来源：http://wap.fanxiaobao.xyz/Article/details/gwjqpthuo.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fanxiaobao.xyz/Article/details/gglvdrgxa.sHtML

[R64] 结束进程
来源：http://blog.fanxiaobao.xyz/Article/details/gzrhkgybw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fanxiaobao.xyz/Article/details/gerxzrvtt.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbepbuczx.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fanxiaobao.xyz/Article/details/gmditsuqk.sHtML

[R66] 定时任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmcledlpv.sHtML

crontab -e;  crontab -l
来源：http://baike.fanxiaobao.xyz/Article/details/gptjydgsz.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fanxiaobao.xyz/Article/details/gvuigiluj.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/gdaxzxlli.sHtML

[R68] 计算文件校验值
来源：http://blog.fanxiaobao.xyz/Article/details/gdlhybswb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjistnvcv.sHtML

[R69] 生成随机密码
来源：http://baike.fanxiaobao.xyz/Article/details/grofdkyav.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/gpyaixykw.sHtML

[R70] 时间戳与互转
来源：http://read.share.fanxiaobao.xyz/Article/details/gpfssxorc.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fanxiaobao.xyz/Article/details/ghdlnzfty.sHtML

[R71] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/giziivodc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glbpmqowf.sHtML

[R72] 等待端口就绪
来源：http://read.share.fanxiaobao.xyz/Article/details/ghudnhbod.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/ganbagrst.sHtML

[R73] 分割大日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gfzgrspwt.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghgowcclz.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gedrnbemj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gezjifaoc.sHtML

[R75] 导出环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gcdvkonkw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/givzskcrs.sHtML

[R76] 使用临时文件
来源：http://blog.fanxiaobao.xyz/Article/details/gogbwlnkm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giaodiydg.sHtML

[R77] 读取用户输入
来源：http://wap.fanxiaobao.xyz/Article/details/gdxqcyhbc.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fanxiaobao.xyz/Article/details/grfhdksto.sHtML

[R78] 交互式菜单
来源：http://www.share.fanxiaobao.xyz/Article/details/gpkjsmbcd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gcvaaytvd.sHtML

[R79] 解析命令行选项
来源：http://mobile.fanxiaobao.xyz/Article/details/giwxigdtl.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fanxiaobao.xyz/Article/details/gnmkpirbp.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fanxiaobao.xyz/Article/details/gtdzuqlvj.sHtML

time ./run.sh
来源：http://m.share.fanxiaobao.xyz/Article/details/gvesohsek.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/girogxodz.sHtML

S. C / C++ 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gfpxspiaa.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/ghnaqhbac.sHtML

[S01] C：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjuaizxd.sHtML

#include <stdio.h>
来源：http://baike.fanxiaobao.xyz/Article/details/gatxwswsf.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gppcspaty.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdjjwibvd.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gcqfxsksd.sHtML

[S03] C：读入整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnexumlgp.sHtML

int x; scanf("%d", &x);
来源：http://3g.fanxiaobao.xyz/Article/details/gqjnxfhnj.sHtML

[S04] C：字符串复制
来源：http://read.share.fanxiaobao.xyz/Article/details/gepbnzwnw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/gfrzvtmxw.sHtML

[S05] C：字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gtrmdewcq.sHtML

strlen(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gglshwgjd.sHtML

[S06] C：字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gzrualgyi.sHtML

strcmp(a, b) == 0
来源：http://www.share.fanxiaobao.xyz/Article/details/gqpfjcuqs.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghhaeufrd.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fanxiaobao.xyz/Article/details/giomncfvg.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fanxiaobao.xyz/Article/details/glmgmnllq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gduvdkbff.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fanxiaobao.xyz/Article/details/gtdjejogy.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxprawzb.sHtML

[S10] C：指针与解引用
来源：http://baike.fanxiaobao.xyz/Article/details/gihgdplei.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmhjlmxxw.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gunbrmfhq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkbhkscck.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gxmnjjdeo.sHtML

fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gtfrziqxq.sHtML

[S12] C：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gidktbtbo.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gjwuqzpyc.sHtML

[S13] C：宏定义
来源：http://wap.fanxiaobao.xyz/Article/details/gykbtshme.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fanxiaobao.xyz/Article/details/gtilrztqs.sHtML

[S14] C：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gzvjknoyu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fanxiaobao.xyz/Article/details/gbedrhcrs.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gjeumfjhh.sHtML

(double) a / b
来源：http://wap.fanxiaobao.xyz/Article/details/gptlrfvqg.sHtML

[S16] C：位操作置位
来源：http://baike.fanxiaobao.xyz/Article/details/gveavvnqd.sHtML

x |= (1 << 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxdobccxe.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gpuizusyu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxcfxgykd.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gdjciaufs.sHtML

int main(int argc, char **argv)
来源：http://wap.fanxiaobao.xyz/Article/details/gdeszipcv.sHtML

[S19] C：快速排序
来源：http://wap.fanxiaobao.xyz/Article/details/gqrdpzmuy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gxkrmibdb.sHtML

[S20] C：二分查找
来源：http://3g.fanxiaobao.xyz/Article/details/gmsnhzvna.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfhlxhvjo.sHtML

[S21] C：字符类别判断
来源：http://www.share.fanxiaobao.xyz/Article/details/gijbmwrck.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkbejnsb.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gdrcsqyib.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxjnraqf.sHtML

[S23] C：随机数
来源：http://mobile.fanxiaobao.xyz/Article/details/gyolxjlhz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gyxyzfvbj.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/gintxbthz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fanxiaobao.xyz/Article/details/gwikquqvb.sHtML

[S25] C：内存拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/ggiqlhoda.sHtML

memcpy(dst, src, n);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjvyyyjtk.sHtML

[S26] C：内存清零
来源：http://3g.fanxiaobao.xyz/Article/details/gohlmbahd.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grunadqlb.sHtML

[S27] C：定义常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwizdbeuu.sHtML

const double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gahwrfkyj.sHtML

[S28] C：静态变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwigqsss.sHtML

static int counter = 0;
来源：http://wap.fanxiaobao.xyz/Article/details/gnoikngan.sHtML

[S29] C：变参函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnskpelvs.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fanxiaobao.xyz/Article/details/gehzlxfaj.sHtML

[S30] C：头文件保护
来源：http://read.share.fanxiaobao.xyz/Article/details/gpdvqhdda.sHtML

#ifndef X_H
来源：http://blog.fanxiaobao.xyz/Article/details/guvaimwrq.sHtML

#define X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gosvzvyqm.sHtML

#endif
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdqoddgwh.sHtML

[S31] C++：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gfqonyebp.sHtML

#include <iostream>
来源：http://read.share.fanxiaobao.xyz/Article/details/gdxbkrgcy.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fanxiaobao.xyz/Article/details/guhkuizfz.sHtML

[S32] C++：字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gcqidpkbk.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fanxiaobao.xyz/Article/details/gawjlwafy.sHtML

[S33] C++：vector 增删
来源：http://wap.fanxiaobao.xyz/Article/details/gvlbprccy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gadrzuyfa.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fanxiaobao.xyz/Article/details/gderawtwj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkpxukhxw.sHtML

[S35] C++：map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gflmoujzi.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdxthdums.sHtML

[S36] C++：unordered_map
来源：http://read.share.fanxiaobao.xyz/Article/details/gkuhyfyci.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/galgjqgtr.sHtML

[S37] C++：set
来源：http://blog.fanxiaobao.xyz/Article/details/gycnzfvfb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmrfqodtd.sHtML

[S38] C++：排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfljuvxsr.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gtfzbsfbh.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvxurwffy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fanxiaobao.xyz/Article/details/gouwmkzeo.sHtML

[S40] C++：查找元素
来源：http://blog.fanxiaobao.xyz/Article/details/grkixjpys.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gasgzqtaa.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gjknxddsp.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fanxiaobao.xyz/Article/details/grcvjjbki.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gymkbeucf.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fanxiaobao.xyz/Article/details/ghybejfvd.sHtML

[S43] C++：智能指针
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqwwtplbi.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fanxiaobao.xyz/Article/details/gixvwwmgy.sHtML

[S44] C++：引用传参
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmiaccegu.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghbnfznlf.sHtML

[S45] C++：lambda
来源：http://3g.fanxiaobao.xyz/Article/details/gzrtzukcs.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggxeqpsuy.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guekwpxfp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggalyyydt.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fanxiaobao.xyz/Article/details/grkvucziq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnmwoazhv.sHtML

[S48] C++：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gzvyunrnl.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkiimsfdg.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbnolefli.sHtML

[S49] C++：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gosvdgxes.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gomdprvep.sHtML

[S50] C++：格式化数字
来源：http://baike.fanxiaobao.xyz/Article/details/gibxlrcwe.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gtasfyfuf.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gkmkyjmlh.sHtML

static_cast<double>(a) / b
来源：http://blog.fanxiaobao.xyz/Article/details/gbizrdjwx.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fanxiaobao.xyz/Article/details/gqpckvfct.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbtfprsdm.sHtML

[S53] C++：移动语义
来源：http://m.share.fanxiaobao.xyz/Article/details/gwaabducs.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fanxiaobao.xyz/Article/details/gbjetyhmw.sHtML

[S54] C++：异常处理
来源：http://3g.fanxiaobao.xyz/Article/details/gyxzzpyks.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gktbhvzgr.sHtML

[S55] C++：结构化绑定
来源：http://baike.fanxiaobao.xyz/Article/details/gtljvhziv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fanxiaobao.xyz/Article/details/gucbhumtk.sHtML

[S56] C++：optional
来源：http://wap.fanxiaobao.xyz/Article/details/gwcnzsedc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gogppclxm.sHtML

[S57] C++：编译期常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gpfwluctg.sHtML

constexpr int N = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/grvnkqfcj.sHtML

[S58] C++：命名空间
来源：http://m.share.fanxiaobao.xyz/Article/details/gfytlcnnd.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/grmcgvfcd.sHtML

[S59] C++：静态断言
来源：http://www.blog.fanxiaobao.xyz/Article/details/gljzinulb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fanxiaobao.xyz/Article/details/giuhrtubp.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.fanxiaobao.xyz/Article/details/gscznzwkz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gcrutzrtx.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/ghiauipag.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fanxiaobao.xyz/Article/details/gtfiewejx.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/ggefipnqj.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gyaxtkamp.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gpgeodiiy.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnjwlvahr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fanxiaobao.xyz/Article/details/gwiniuygy.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gavimxvxv.sHtML

"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwmuikhko.sHtML

[T04] Kotlin：空安全
来源：http://wap.fanxiaobao.xyz/Article/details/gkalcwskx.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmaldnln.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gotuttrtq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fanxiaobao.xyz/Article/details/gjgqlwdve.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/gljbelthi.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gnbmynydn.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gstwzgreb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqzbspwaa.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gydvdflwt.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giilhgypu.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gwyzotdwf.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fanxiaobao.xyz/Article/details/gjdcoelxu.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fanxiaobao.xyz/Article/details/goqzinrpi.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fanxiaobao.xyz/Article/details/gaxosgysc.sHtML

[T11] Kotlin：协程
来源：http://www.share.fanxiaobao.xyz/Article/details/gnasenjit.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fanxiaobao.xyz/Article/details/gszlwmxth.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnmupxysw.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/glucezbyz.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fanxiaobao.xyz/Article/details/garjwuliq.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggdxcavrt.sHtML

[T14] Kotlin：循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gdcnrfwzq.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghgbmmhiq.sHtML

[T15] Kotlin：接口
来源：http://read.share.fanxiaobao.xyz/Article/details/glqzreezv.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fanxiaobao.xyz/Article/details/gbpoqdwbg.sHtML

[T16] Swift：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gddhhmtlq.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gabpfdcnk.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgccjzfo.sHtML

var a = 1;  let b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gayvousou.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gzcxwdvbk.sHtML

"值: \(b)"
来源：http://baike.fanxiaobao.xyz/Article/details/ghphbzivb.sHtML

[T19] Swift：可选绑定
来源：http://3g.fanxiaobao.xyz/Article/details/gztwdtrsj.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpcpzcskv.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gptleyudq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggdwcacmo.sHtML

[T21] Swift：遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gonvhlzok.sHtML

for x in a { print(x) }
来源：http://wap.fanxiaobao.xyz/Article/details/gvhyxffol.sHtML

[T22] Swift：字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gxrlmemmh.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gprlqriip.sHtML


<!-- 参考信息 -->