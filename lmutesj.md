代发 wailian999

echo $((1 + 2 * 3))
来源：http://read.share.zdbjq.cn/Article/details/gwddtuyuz.sHtML

[R28] 浮点运算
来源：http://www.blog.zdbjq.cn/Article/details/gsmkwaedm.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fehbvm.com/Article/details/gfvrwsahf.sHtML

[R29] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/gltcookfg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fehbvm.com/Article/details/gwgmrphrt.sHtML

[R30] 函数返回状态码
来源：http://www.share.zdbjq.cn/Article/details/gsyjmwshu.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.zdbjq.cn/Article/details/gxxyylbiy.sHtML

[R31] 局部变量
来源：http://mobile.fehbvm.com/Article/details/getdtsrrk.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.hesvh.cn/Article/details/gumbtibvf.sHtML

[R32] 参数个数校验
来源：http://mobile.hesvh.cn/Article/details/gikdquzyc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/gvkplczjc.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.zdbjq.cn/Article/details/gvfpplhfg.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fehbvm.com/Article/details/gimvxcpsd.sHtML

[R34] 退出时清理
来源：http://read.share.zdbjq.cn/Article/details/gpryclxlj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gzhbvftge.sHtML

[R35] 后台执行并等待
来源：http://www.share.zdbjq.cn/Article/details/gtjvhebbi.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.hesvh.cn/Article/details/gzivpvnhm.sHtML

[R36] 并发执行多个任务
来源：http://blog.zdbjq.cn/Article/details/grbeuqlvp.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.zdbjq.cn/Article/details/gohurmdde.sHtML

[R37] 把输出赋给变量
来源：http://baike.hesvh.cn/Article/details/gjewhvfdb.sHtML

files=$(ls -1)
来源：http://www.blog.zdbjq.cn/Article/details/gqeawvjwz.sHtML

[R38] 管道串联
来源：http://read.share.hesvh.cn/Article/details/ggccvdeit.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fehbvm.com/Article/details/guwqgqyqi.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.zdbjq.cn/Article/details/gzucoundw.sHtML

cmd > out.log 2>&1
来源：http://3g.zdbjq.cn/Article/details/gixbernso.sHtML

[R40] 追加写日志
来源：http://www.blog.hesvh.cn/Article/details/gnwjoxlgg.sHtML

echo "log" >> out.log
来源：http://read.share.hesvh.cn/Article/details/gdmkpbvxx.sHtML

[R41] 丢弃输出
来源：http://read.share.zdbjq.cn/Article/details/gpgedyger.sHtML

cmd >/dev/null 2>&1
来源：http://wap.hesvh.cn/Article/details/gtlngifru.sHtML

[R42] 输入重定向
来源：http://baike.zdbjq.cn/Article/details/gjhmyyptg.sHtML

wc -l < a.txt
来源：http://blog.hesvh.cn/Article/details/gsnaipeja.sHtML

[R43] 按名字查找文件
来源：http://mobile.fehbvm.com/Article/details/grpxmmqvj.sHtML

find . -name "*.log" -type f
来源：http://blog.zdbjq.cn/Article/details/glncyihfr.sHtML

[R44] 按修改时间查找
来源：http://m.share.fehbvm.com/Article/details/gglkmnavb.sHtML

find . -mtime -7 -type f
来源：http://baike.hesvh.cn/Article/details/ggsbfxdik.sHtML

[R45] 批量删除
来源：http://baike.fehbvm.com/Article/details/gvbijzhcr.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fehbvm.com/Article/details/gsvhmdqmt.sHtML

[R46] 递归替换文件内容
来源：http://3g.fehbvm.com/Article/details/gxjvizvhv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.zdbjq.cn/Article/details/gnpravlgo.sHtML

[R47] sed 单行替换
来源：http://m.share.zdbjq.cn/Article/details/gfpzmbyiw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fehbvm.com/Article/details/gvqpjjlxf.sHtML

[R48] awk 取指定列
来源：http://blog.zdbjq.cn/Article/details/gjqqajjdm.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fehbvm.com/Article/details/gkghobdsa.sHtML

[R49] awk 带条件
来源：http://mobile.fehbvm.com/Article/details/ghhkvnleu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.hesvh.cn/Article/details/gayrwaedq.sHtML

[R50] awk 求和
来源：http://mobile.fehbvm.com/Article/details/gagxstple.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gjtbwildu.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fehbvm.com/Article/details/gshbzwylo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fehbvm.com/Article/details/gzahfsyhx.sHtML

[R52] 统计行数
来源：http://www.blog.hesvh.cn/Article/details/ghdtppfhk.sHtML

wc -l a.txt
来源：http://www.share.hesvh.cn/Article/details/gbtiucvro.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.zdbjq.cn/Article/details/gjkmyklyz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.hesvh.cn/Article/details/gysxxkulq.sHtML

[R54] 比较两个文件
来源：http://www.share.hesvh.cn/Article/details/grfgopmbq.sHtML

diff a.txt b.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gtdnbmucu.sHtML

[R55] 压缩与解压
来源：http://www.m.share.zdbjq.cn/Article/details/gvgptifno.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fehbvm.com/Article/details/gwuetiqxm.sHtML

[R56] 远程拷贝
来源：http://blog.hesvh.cn/Article/details/gvndkeyxs.sHtML

scp file user@host:/path/
来源：http://www.blog.zdbjq.cn/Article/details/ggofhtkvt.sHtML

[R57] 远程执行命令
来源：http://3g.hesvh.cn/Article/details/gzphbxgsa.sHtML

ssh user@host 'uptime'
来源：http://baike.hesvh.cn/Article/details/gvlxjlxdj.sHtML

[R58] 下载文件
来源：http://3g.fehbvm.com/Article/details/gatogtryj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.zdbjq.cn/Article/details/gcjkgxbmc.sHtML

[R59] 发 POST JSON
来源：http://baike.fehbvm.com/Article/details/guldlqfxx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.zdbjq.cn/Article/details/gogczkovh.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.hesvh.cn/Article/details/gxmelggmk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.hesvh.cn/Article/details/gqtighrpr.sHtML

[R61] 磁盘占用
来源：http://read.share.hesvh.cn/Article/details/gizowzioj.sHtML

df -h;  du -sh *
来源：http://m.share.zdbjq.cn/Article/details/gvvjaajfx.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fehbvm.com/Article/details/gfnshcvii.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fehbvm.com/Article/details/ghpmtszlo.sHtML

[R63] 内存与进程
来源：http://www.blog.zdbjq.cn/Article/details/geexrrilz.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.zdbjq.cn/Article/details/gzgierspc.sHtML

[R64] 结束进程
来源：http://www.m.share.hesvh.cn/Article/details/gxzativio.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.zdbjq.cn/Article/details/gqrtdesuk.sHtML

[R65] 查看端口占用
来源：http://mobile.fehbvm.com/Article/details/gabvircag.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.zdbjq.cn/Article/details/gmevwfuer.sHtML

[R66] 定时任务
来源：http://wap.zdbjq.cn/Article/details/ghlqzrttf.sHtML

crontab -e;  crontab -l
来源：http://3g.zdbjq.cn/Article/details/gxazcelsq.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.hesvh.cn/Article/details/ginhvjewe.sHtML

openssl rand -hex 16
来源：http://www.m.share.fehbvm.com/Article/details/gpfdljobq.sHtML

[R68] 计算文件校验值
来源：http://mobile.hesvh.cn/Article/details/gfwtpdddg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fehbvm.com/Article/details/gebatuoww.sHtML

[R69] 生成随机密码
来源：http://www.m.share.hesvh.cn/Article/details/gaxmrifoc.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fehbvm.com/Article/details/glverthhk.sHtML

[R70] 时间戳与互转
来源：http://3g.hesvh.cn/Article/details/gsuwjbupa.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fehbvm.com/Article/details/glbpidiot.sHtML

[R71] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/gbxovyljh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.hesvh.cn/Article/details/gefbzuqtd.sHtML

[R72] 等待端口就绪
来源：http://read.share.hesvh.cn/Article/details/gypyituau.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/gyaugcugw.sHtML

[R73] 分割大日志
来源：http://baike.zdbjq.cn/Article/details/gigbywqyu.sHtML

split -l 1000 big.log part_
来源：http://blog.zdbjq.cn/Article/details/gydttjigt.sHtML

[R74] 批量重命名
来源：http://www.m.share.hesvh.cn/Article/details/guefjdggm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.zdbjq.cn/Article/details/gxbtkfdgi.sHtML

[R75] 导出环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gqebovtod.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fehbvm.com/Article/details/gjgmztqpc.sHtML

[R76] 使用临时文件
来源：http://www.blog.fehbvm.com/Article/details/gfehghjzc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/gjmxrgbfx.sHtML

[R77] 读取用户输入
来源：http://www.blog.zdbjq.cn/Article/details/gnrnmexpw.sHtML

read -rp "请输入: " ans
来源：http://3g.hesvh.cn/Article/details/gedcotngx.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fehbvm.com/Article/details/gkaccydvw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.zdbjq.cn/Article/details/gsuyckiec.sHtML

[R79] 解析命令行选项
来源：http://baike.zdbjq.cn/Article/details/gpmawkneh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.hesvh.cn/Article/details/gtcazlbid.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.hesvh.cn/Article/details/gqwwxngsb.sHtML

time ./run.sh
来源：http://baike.fehbvm.com/Article/details/gmvphuaan.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gkxiekvpa.sHtML

S. C / C++ 专题
来源：http://read.share.fehbvm.com/Article/details/gbunprddw.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gqqugxguu.sHtML

[S01] C：Hello World
来源：http://read.share.fehbvm.com/Article/details/gwtbeduyo.sHtML

#include <stdio.h>
来源：http://read.share.zdbjq.cn/Article/details/ghodukzgp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fehbvm.com/Article/details/gmslblypw.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.hesvh.cn/Article/details/gcspdxzqr.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fehbvm.com/Article/details/gwnfpyjrw.sHtML

[S03] C：读入整数
来源：http://read.share.hesvh.cn/Article/details/gaqgozybu.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.hesvh.cn/Article/details/ggolwjmxo.sHtML

[S04] C：字符串复制
来源：http://3g.fehbvm.com/Article/details/gxwwdnkfq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.zdbjq.cn/Article/details/gztulyxno.sHtML

[S05] C：字符串长度
来源：http://blog.hesvh.cn/Article/details/gunlcirtk.sHtML

strlen(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gyixwjjxn.sHtML

[S06] C：字符串比较
来源：http://www.blog.hesvh.cn/Article/details/grdbadgys.sHtML

strcmp(a, b) == 0
来源：http://mobile.fehbvm.com/Article/details/gznsotpkn.sHtML

[S07] C：数组遍历求和
来源：http://3g.zdbjq.cn/Article/details/gpwbjgipb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.hesvh.cn/Article/details/gnlwznaon.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.zdbjq.cn/Article/details/gxzfbehus.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fehbvm.com/Article/details/gijxpcxlo.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fehbvm.com/Article/details/gyicyoztj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.hesvh.cn/Article/details/gvvzmqtkb.sHtML

[S10] C：指针与解引用
来源：http://read.share.hesvh.cn/Article/details/gfchcizoo.sHtML

int *p = &a;  *p = 5;
来源：http://wap.hesvh.cn/Article/details/gdyteqejl.sHtML

[S11] C：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/giyyhaunj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fehbvm.com/Article/details/gxfjdkllx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fehbvm.com/Article/details/gkbmozsak.sHtML

fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/goxhceoeg.sHtML

[S12] C：写文件
来源：http://3g.zdbjq.cn/Article/details/gyhlkcuzm.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/gahlhkeah.sHtML

[S13] C：宏定义
来源：http://mobile.fehbvm.com/Article/details/gwabbldzj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.zdbjq.cn/Article/details/gfdocjbmj.sHtML

[S14] C：枚举
来源：http://www.m.share.fehbvm.com/Article/details/gmcvopgpy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.zdbjq.cn/Article/details/gdsulwfkb.sHtML

[S15] C：类型转换
来源：http://read.share.hesvh.cn/Article/details/gfcnbryvx.sHtML

(double) a / b
来源：http://m.share.zdbjq.cn/Article/details/gudxyncbn.sHtML

[S16] C：位操作置位
来源：http://mobile.zdbjq.cn/Article/details/gvbttndti.sHtML

x |= (1 << 3);
来源：http://www.blog.hesvh.cn/Article/details/gbyghidxu.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fehbvm.com/Article/details/gcztqteve.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fehbvm.com/Article/details/gpcayremn.sHtML

[S18] C：命令行参数
来源：http://mobile.fehbvm.com/Article/details/gsionpowm.sHtML

int main(int argc, char **argv)
来源：http://baike.hesvh.cn/Article/details/githrcelq.sHtML

[S19] C：快速排序
来源：http://m.share.hesvh.cn/Article/details/gzcfulemx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gcaunqnbs.sHtML

[S20] C：二分查找
来源：http://www.blog.zdbjq.cn/Article/details/gngrcwmjh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/gkwlsqmch.sHtML

[S21] C：字符类别判断
来源：http://mobile.fehbvm.com/Article/details/gbhpbuacn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.hesvh.cn/Article/details/glrfdiabz.sHtML

[S22] C：字符串转数字
来源：http://m.share.hesvh.cn/Article/details/gmuqkczki.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.hesvh.cn/Article/details/gqlnedsrc.sHtML

[S23] C：随机数
来源：http://www.blog.fehbvm.com/Article/details/gpqpezvdv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.zdbjq.cn/Article/details/gumjihkml.sHtML

[S24] C：获取本地时间
来源：http://www.share.zdbjq.cn/Article/details/gamgkcepx.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.zdbjq.cn/Article/details/gyvjvxczy.sHtML

[S25] C：内存拷贝
来源：http://mobile.fehbvm.com/Article/details/grjoblzll.sHtML

memcpy(dst, src, n);
来源：http://blog.fehbvm.com/Article/details/gwiuxsfuh.sHtML

[S26] C：内存清零
来源：http://www.blog.zdbjq.cn/Article/details/gzgfeplyl.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.hesvh.cn/Article/details/gdqowcnaw.sHtML

[S27] C：定义常量
来源：http://3g.hesvh.cn/Article/details/gvwlzmkta.sHtML

const double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gtrkkkmnt.sHtML

[S28] C：静态变量
来源：http://www.blog.zdbjq.cn/Article/details/gjlniagfz.sHtML

static int counter = 0;
来源：http://blog.hesvh.cn/Article/details/gsabaiymk.sHtML

[S29] C：变参函数
来源：http://www.share.zdbjq.cn/Article/details/gqdomxwwe.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.zdbjq.cn/Article/details/grkugvwos.sHtML

[S30] C：头文件保护
来源：http://blog.hesvh.cn/Article/details/gknmyesdc.sHtML

#ifndef X_H
来源：http://www.share.zdbjq.cn/Article/details/gpzmxdmrb.sHtML

#define X_H
来源：http://read.share.hesvh.cn/Article/details/gkwlzmwdu.sHtML

#endif
来源：http://www.blog.zdbjq.cn/Article/details/gkjdaokpm.sHtML

[S31] C++：Hello World
来源：http://baike.zdbjq.cn/Article/details/gzyejxulr.sHtML

#include <iostream>
来源：http://www.blog.zdbjq.cn/Article/details/gtozlnxgk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fehbvm.com/Article/details/giispznsi.sHtML

[S32] C++：字符串
来源：http://mobile.fehbvm.com/Article/details/gnaogqfpk.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fehbvm.com/Article/details/gkqtctyfz.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.hesvh.cn/Article/details/gnukjeecr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.hesvh.cn/Article/details/groyikhkz.sHtML

[S34] C++：遍历 vector
来源：http://baike.hesvh.cn/Article/details/grrhnkyli.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fehbvm.com/Article/details/ghbpjzpli.sHtML

[S35] C++：map
来源：http://www.share.zdbjq.cn/Article/details/gvmheelun.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gopckoiks.sHtML

[S36] C++：unordered_map
来源：http://mobile.fehbvm.com/Article/details/gllenunsi.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gptsjtrty.sHtML

[S37] C++：set
来源：http://www.blog.zdbjq.cn/Article/details/gtjaexlom.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.zdbjq.cn/Article/details/geyxioehz.sHtML

[S38] C++：排序
来源：http://www.m.share.zdbjq.cn/Article/details/glmmhubjg.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fehbvm.com/Article/details/gcuabkebs.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.hesvh.cn/Article/details/gfducovil.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.hesvh.cn/Article/details/gsebukiwj.sHtML

[S40] C++：查找元素
来源：http://wap.zdbjq.cn/Article/details/gobocrqno.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fehbvm.com/Article/details/ghfdvsleq.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gcqgmfhgh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fehbvm.com/Article/details/gvskxjtuj.sHtML

[S42] C++：继承与虚函数
来源：http://blog.zdbjq.cn/Article/details/gmaaglwtb.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.zdbjq.cn/Article/details/ggnoispxo.sHtML

[S43] C++：智能指针
来源：http://wap.hesvh.cn/Article/details/gzckqxpwf.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.hesvh.cn/Article/details/gavlbiluk.sHtML

[S44] C++：引用传参
来源：http://www.blog.zdbjq.cn/Article/details/gkezpftza.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.hesvh.cn/Article/details/gwlxndjrp.sHtML

[S45] C++：lambda
来源：http://www.blog.zdbjq.cn/Article/details/glkuotdib.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.hesvh.cn/Article/details/ghbgnqwea.sHtML

[S46] C++：函数模板
来源：http://www.m.share.zdbjq.cn/Article/details/ggwzbtwyh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.zdbjq.cn/Article/details/glpfqmrgi.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fehbvm.com/Article/details/gghuljjvd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.zdbjq.cn/Article/details/gbfawjgzr.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gnmxlrprz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.zdbjq.cn/Article/details/gtrjqosse.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.zdbjq.cn/Article/details/gzqqpqmgy.sHtML

[S49] C++：写文件
来源：http://3g.hesvh.cn/Article/details/gmwwhlbwt.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.hesvh.cn/Article/details/ghngmqerh.sHtML

[S50] C++：格式化数字
来源：http://www.share.fehbvm.com/Article/details/gevlpjypy.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gshiuwygu.sHtML

[S51] C++：显式类型转换
来源：http://mobile.zdbjq.cn/Article/details/gmqkpxjtu.sHtML

static_cast<double>(a) / b
来源：http://blog.zdbjq.cn/Article/details/gaamiytgr.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.zdbjq.cn/Article/details/gguelqacy.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.hesvh.cn/Article/details/gywqhrzei.sHtML

[S53] C++：移动语义
来源：http://m.share.zdbjq.cn/Article/details/gnqixuubo.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fehbvm.com/Article/details/gcbvadoat.sHtML

[S54] C++：异常处理
来源：http://www.blog.fehbvm.com/Article/details/glixunwqn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fehbvm.com/Article/details/gvedrrpdm.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.zdbjq.cn/Article/details/guqyxmtjk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.zdbjq.cn/Article/details/gfqjlswip.sHtML

[S56] C++：optional
来源：http://baike.zdbjq.cn/Article/details/gkbzaejfv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.hesvh.cn/Article/details/gpoeltzbb.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.hesvh.cn/Article/details/gnwujbewc.sHtML

constexpr int N = 10;
来源：http://m.share.hesvh.cn/Article/details/goedbrhlw.sHtML

[S58] C++：命名空间
来源：http://3g.zdbjq.cn/Article/details/gyqxgdoyc.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.hesvh.cn/Article/details/gjiwkcpat.sHtML

[S59] C++：静态断言
来源：http://blog.hesvh.cn/Article/details/gpmgyyttq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.hesvh.cn/Article/details/glfbxlham.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.hesvh.cn/Article/details/gdqqoekat.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gjcsvxugw.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gqvdxabhv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.hesvh.cn/Article/details/gtwmwplod.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gocvbejbd.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.hesvh.cn/Article/details/gzswpjnsl.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/grkeyxjfy.sHtML

[T02] Kotlin：变量
来源：http://mobile.fehbvm.com/Article/details/gxnhhoocl.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.zdbjq.cn/Article/details/geflfqxgb.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.zdbjq.cn/Article/details/gqivlnkcp.sHtML

"值: $b"
来源：http://m.share.hesvh.cn/Article/details/gfljoughk.sHtML

[T04] Kotlin：空安全
来源：http://blog.zdbjq.cn/Article/details/gvwbyyrnl.sHtML

val n: String? = null;  n?.length
来源：http://www.share.zdbjq.cn/Article/details/gjxsuxjdd.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.hesvh.cn/Article/details/gtifrufki.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.hesvh.cn/Article/details/gbwqsflpb.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fehbvm.com/Article/details/glgrydocy.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gxscwxtpq.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fehbvm.com/Article/details/gzbhxczul.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.zdbjq.cn/Article/details/gbappdgio.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fehbvm.com/Article/details/gqqgijsgg.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fehbvm.com/Article/details/ghnuzptin.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.zdbjq.cn/Article/details/gygvwgfue.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.zdbjq.cn/Article/details/glivufzgo.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.zdbjq.cn/Article/details/ggopwcujw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.hesvh.cn/Article/details/gtgarrkou.sHtML

[T11] Kotlin：协程
来源：http://wap.hesvh.cn/Article/details/gxegksmqx.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.hesvh.cn/Article/details/gtmmwtmht.sHtML

[T12] Kotlin：解构声明
来源：http://blog.zdbjq.cn/Article/details/ggzxfcmds.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gmvbtafku.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.zdbjq.cn/Article/details/glhmrvura.sHtML

val m = mapOf("a" to 1)
来源：http://baike.zdbjq.cn/Article/details/gzqrbvlib.sHtML

[T14] Kotlin：循环
来源：http://blog.fehbvm.com/Article/details/gjrfstdhs.sHtML

for (i in 1..10) println(i)
来源：http://3g.zdbjq.cn/Article/details/gypxwynvh.sHtML

[T15] Kotlin：接口
来源：http://m.share.hesvh.cn/Article/details/gsoxqrlej.sHtML

interface Shape { fun area(): Double }
来源：http://3g.hesvh.cn/Article/details/gjojetfzm.sHtML

[T16] Swift：Hello World
来源：http://baike.hesvh.cn/Article/details/gekwsnpzg.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/gmnergzok.sHtML

[T17] Swift：变量与常量
来源：http://blog.hesvh.cn/Article/details/gjrgheogh.sHtML

var a = 1;  let b = 2
来源：http://www.blog.hesvh.cn/Article/details/gqiwxxrrz.sHtML

[T18] Swift：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gpykyzeuk.sHtML

"值: \(b)"
来源：http://blog.fehbvm.com/Article/details/gdwitbmzo.sHtML

[T19] Swift：可选绑定
来源：http://baike.hesvh.cn/Article/details/gebtpbfmi.sHtML

if let n = opt { print(n) }
来源：http://www.blog.hesvh.cn/Article/details/gdywashjn.sHtML

[T20] Swift：数组操作
来源：http://baike.fehbvm.com/Article/details/gpzudxthv.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fehbvm.com/Article/details/gnnhhrdeu.sHtML

[T21] Swift：遍历
来源：http://3g.fehbvm.com/Article/details/gwcnnycti.sHtML

for x in a { print(x) }
来源：http://wap.fehbvm.com/Article/details/ghpxocwpf.sHtML

[T22] Swift：字典
来源：http://www.m.share.fehbvm.com/Article/details/gecmmdtuv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fehbvm.com/Article/details/gmncdthtb.sHtML

[T23] Swift：函数
来源：http://m.share.hesvh.cn/Article/details/gynacspqa.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fehbvm.com/Article/details/gmwwuagjq.sHtML

[T24] Swift：闭包
来源：http://www.share.hesvh.cn/Article/details/gnxplwtwm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.hesvh.cn/Article/details/greumindh.sHtML

[T25] Swift：结构体
来源：http://wap.hesvh.cn/Article/details/gnimxkjak.sHtML

struct P { var x: Int }
来源：http://www.m.share.hesvh.cn/Article/details/gkhaiytxt.sHtML

[T26] Swift：类与重写
来源：http://3g.zdbjq.cn/Article/details/gowwgvzpc.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fehbvm.com/Article/details/ghukqzqzy.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fehbvm.com/Article/details/gsubdewte.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fehbvm.com/Article/details/gyxrqqcfi.sHtML

[T28] Swift：枚举
来源：http://read.share.hesvh.cn/Article/details/gyvguqpyw.sHtML

enum Color { case red, green }
来源：http://read.share.fehbvm.com/Article/details/gqucllpdh.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fehbvm.com/Article/details/ghlnbsegk.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fehbvm.com/Article/details/gfnjjivhw.sHtML

[T30] Swift：协议
来源：http://read.share.fehbvm.com/Article/details/grhebyckq.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.zdbjq.cn/Article/details/gyxwpuovp.sHtML


<!-- 参考信息 -->