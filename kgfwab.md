代发 wailian999

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2flozbtck.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2wfnfgnqh.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2desqjmti.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ndwmllmo.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2ioxwhaxo.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2jwaimyxp.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2wslxgbgs.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2zlqylzqf.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2vodausyp.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2lmrrdidg.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2cjgntrgx.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2rohqtzkx.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2yfmneaqe.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2ziwjbqgg.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2ylnzoaey.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2exvwlipq.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2ugorpgml.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2xonpisga.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2sbojtknb.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2cdqsctet.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2krypnluu.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2svvenwou.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2bzdfnyag.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2xtlutscf.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2froygczr.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2ezabjqjg.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2xxouxdlj.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2szkrgtey.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2lwgartih.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2lhwxgtgh.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2uzuezbxs.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2bkftpzcg.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2dsdwxyej.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2dcbfknzk.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2sxaqhqtk.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2tytjcvfk.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2enzaoghv.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2kpzhhwed.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2mtoysony.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2kepjejxg.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2coibiqhu.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2osgalhbm.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2isrrvfcp.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2olanzkng.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2ptdgncwr.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2pydjctmy.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2buafsrbl.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2bvzqhowq.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2scnunbdh.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2wbcwaynw.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2moaxylfg.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2orkzyzeo.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2huhavsis.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2rgbavdss.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2amxwbgfr.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2ufhxukju.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2avppqpcs.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2plodctkv.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2sqmaonpj.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2suhzgfzo.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2paxcyize.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2yxeslevy.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wbpkvxqs.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2cpxnugzu.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2apmnssgf.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2naziqrvv.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2ncfxwjhh.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2vlhtgtbb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2lzfptpor.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2tqlcfwur.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rolixnbt.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2kuspuigs.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2oowvhmpe.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2einqwrym.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2qccqnony.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2oerreywe.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2ufkiulrx.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2nzkyoxaz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2jsbcaygj.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2aqolicsk.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2krdxuysh.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2rfqdxhrw.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2bcfnkktb.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2epzmkost.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2szlsdlaq.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2fcafjzuc.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2kcdreoda.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2oftbbuyv.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2hznusfns.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2ypoyefio.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2zmdamdke.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2qnpnayop.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2oyvwypld.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2cagedoaj.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2ovvopibr.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2bysfyiak.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2nsvzibkh.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2mfptoygq.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2mmxehlja.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2atyluhjh.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2nvfchett.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2fwhabfuf.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2zlfpzidz.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2jvmkvacs.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2ibrmrqgm.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2nrsgoynv.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2xmmczcye.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2kwnnxugk.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2ffallqil.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2nrvphviy.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2eehmnlou.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2wupbnazr.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2yofjbhhc.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2pjasacnm.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2rjlzbhym.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2ziknoisy.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2xofjtyow.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2mfptkeen.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2tylwefga.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2gsuddeqq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2pxwxcknf.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2umdqnvel.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2pjfzmcta.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cihibsof.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2bmdjpfxm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nahxasot.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2msfprmbc.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2kykjwlip.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2ywldvobv.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2womzpcfn.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2qglutwiq.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2xhxeuwko.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2cbeelgym.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2zkxejuwi.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2fdahkyoh.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2jvulmaeq.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gnsgfcod.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2uphtwxog.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2ldjtksxa.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2yvwewbre.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2vpvlltux.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2posapslq.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2uxpuefdq.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2loahuswe.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2kxxsiaws.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2mihwbvnr.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2xrjwjeiy.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2wbikokjj.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2mixejmbp.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2obnrmzls.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2eqlcopxd.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2fiexviyt.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2ozttuusz.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2pbgetwea.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2fcjkigxv.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2nfdkfkjv.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2ljdcmxnc.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2vsszvgyj.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2ocoynhvv.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2bfvihcns.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2mmuxtaej.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2tdfirxim.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2xxdvlezc.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2vzjplqxg.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2vekbgxnr.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2npcvnjli.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2gamjcagp.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2yudobrpx.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2aqwgexgb.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2eopyawxs.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2kogibvuc.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2omyspmwf.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2rpddbaft.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2wljsegyb.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2otolkbwm.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2wrgdlpmr.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2bbkwttjc.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2kumowuyr.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2ziashjtr.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2uwmyhrzk.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2dvotmlcu.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2badhrxnf.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2uiowjotx.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2rkrylqed.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2zcupjtnb.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2kymrwumx.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2kddiljfw.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2ydirivmg.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2ytlleogy.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2cnqnnrai.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2kjedlppz.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2djyavtkh.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2ajffabtf.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2tboyvirk.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wtumljem.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2epmzsvjh.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2yklelkmc.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2qexfgorm.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2prdinpbr.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2qxsvbhls.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2zrmhzbpi.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2deagyxmw.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2hwqkusuz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2lvdhgsqa.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2kuqkvvis.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2tzhocbdb.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2jbpnkhoo.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2weptpovb.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2yfwthraj.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2jnyhuidp.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2mhbyavgm.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lymorxbn.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2tavrxynr.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2whyffpkc.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2fkrdbmba.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2nwanulmv.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2dppfqgol.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2xaauqtss.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2gsjaffjf.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2dpazmolg.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2uxysnawi.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2fhfyzfim.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2wdsysiei.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2snnrtujc.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hvauhvbs.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2hxidreyb.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2rvnscrzs.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2qgsvqepc.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2gurwuqin.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2iqjkleta.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2nyrwsybv.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2hfcqlzpl.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2lgjvwpxi.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2xwbuhvqk.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2tsblalfa.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2xkrvleuk.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2ykxveptm.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2dbxycufk.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2mxcbffvs.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2niuzmtsk.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2fucgconv.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2bgcywbii.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ettihdur.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2zgvhyctr.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2mjndwyuz.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2gosjoewy.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2wcnzjllm.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2ssaeyqfd.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2gjldcgyd.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2qioyluny.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2lfbrwwzi.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2cqkjwvvx.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2znbbylwe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fidzzwtb.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2xrklwbio.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2blhvkgnp.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mhmtufau.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2cpbzukcc.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2aahswdow.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2rgjhkrck.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2ianifbfx.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2smykfgid.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2mmbwxkqy.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2zkmiuimf.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2zcykyjfk.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2snpxbhyy.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2nmmymtgr.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2bacsvrij.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2xwnibmzx.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2yrkfgvwl.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2mmfgrgzz.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2mhjrlqpq.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2cwsbtabr.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2xvcxoknf.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2urdgaqys.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2esicigwh.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2philylam.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2whyowyly.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2ddqryjez.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2qhsroztl.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2hwagwhjb.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2lhfjtwwo.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2fqlocdxa.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ggqjfruo.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2ejybnans.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2vmdjotoc.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2pjvtabnk.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2mpbjevzy.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2wjemfebc.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2tacdwxxd.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2radbzzlt.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2yypuabam.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2xejieipn.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2lqnlgnhj.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2clbukztf.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2ixjxnscj.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2xxdgmcad.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2jxfwiqxk.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2hjignumc.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2mxktbanw.html


<!-- 参考信息 -->