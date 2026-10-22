代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2twuweiba.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2bkqpznnm.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2nailbnjy.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2vxxllgdt.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2sxamonko.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2cvyxnwvj.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2thlantqz.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2hfmcdntb.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2dkrsfaue.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2yokzlgsj.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2zmiecyqi.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2unowrkxw.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rbvepfyc.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2gnpuaszs.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2yizfkgko.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2zhmvhota.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2dasvnmpm.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2mfwtmqvl.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2ldvrskwx.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2nvkrszck.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2anfycqih.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2ivtlrjjo.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2ctkvjfyz.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2gsbmjmyr.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2aqljcxay.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2qtidxfjt.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2wzpqzcwn.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2qmapnkit.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2yntubnyq.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2mbeqooec.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2xjzoqhos.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2uslkdrmi.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2juzandqm.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2btyjtsvi.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2bgqvipwv.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2lffejdza.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2xufpaoub.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2yzcuysro.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ozicyqap.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2cbslpnfi.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2zosctgzm.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2jbuezzfc.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2tfkinmrb.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2xrlhntxx.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2jddziwnq.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2oajtxpdl.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2czfybfkd.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2snmezmvz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2xocdsnrj.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2phedbsxo.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2dclfwibx.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2qrwfwusp.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2tkkqmwom.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2cyoucnwr.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2rijgaekx.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2qvmhiliq.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2nmzworsl.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ohucxbni.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2qiyqhrvk.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2lfvbctgw.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2reldpugs.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2zbribkyx.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2hfaxgqnt.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2byarasnb.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2yubpzlfz.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2rtbhgyyi.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2msisgazu.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2gvuypycb.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2iwciltti.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2kvftgzim.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2qzjfjbrw.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2vqeiilxg.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2klmuuzis.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2dqgunkei.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2zyjdyowr.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2tqmlaehk.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2hciexhyb.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2kjkdjocs.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2dthyzcda.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2ajtkwnwz.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2eufixaxy.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2jxgfnwcj.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2aecbcras.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2unycukrr.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2jlcsxury.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2wcswohal.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2njoeylgf.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2siwkdhhf.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2qxmeiplx.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2bdqvgikt.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2nmckrrbj.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2pkkyouvg.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2bbckyote.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2ucqupnlw.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2oomxtymp.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2zljpvhsi.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2fhiqdhqd.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2sanopejb.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2dmsqdote.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2gslwnibf.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2eyqdoxtz.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2fhdjpooa.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2vpfbwilz.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2owphurta.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2lqrxifck.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2gwxwdsfz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2jedczdqf.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2bydfgizm.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2dgxxijpx.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2mvuulswo.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2odhpkayl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2suiqnxpu.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2ybjubkhp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bsqphcrx.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tadbdhkl.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2qcbehckl.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2vxpdhaps.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2tzejiqmq.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2pgtynect.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2ryyvrvbi.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2rzvmpapi.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2agojnbjx.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2zwslnsxe.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2cgasimab.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2suftanpk.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2szdvbwzp.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2finqqbea.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2mvjpmnwd.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2bwmxtjfk.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2roflahcr.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2ncguxilb.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2tngcezuc.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2ggidepir.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2bpzwfupt.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2pgcgtiap.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ancpislm.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2uyhtgrlg.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2pdbgwpma.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2hygidltp.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2lkzrphcv.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2zgnthldo.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2xymrfinm.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2eveibtut.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2npejnivh.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2jwqxaido.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2ljiacdjp.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2oxlrrtah.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2qvavcfok.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2wzqgwdqa.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rjthcpcc.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2wbkpwocj.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2sjnmumjx.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2krskcebp.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2nefmzoih.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2plkejqjo.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2eoxehowm.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2hwovavif.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2npagtdvy.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2oflgpqmz.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2twputxyo.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2atjmznuv.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2zmwnptxf.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2mapnklzc.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2aojvnrfc.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2cjneplrg.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2opthcxbu.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2mnjflpky.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2nlashulw.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2xnwrwnpl.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2plashvcn.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2oaylvgok.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2rkekedco.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2xvqkvafv.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2lxngwwym.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2nqavxhch.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2bytjvtga.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2dpsaoqtv.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2ycpoafpi.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2wossccfp.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rdrrkmql.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2vqdqnffi.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2argvjgei.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2zvjrcsjo.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2toitshis.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2nmsoevpy.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2rflrmmye.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2bgtgtxzd.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2pennpbep.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2rypwtvrh.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2uxbmyarf.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2fouxbagc.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2bhdmxopc.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2nrbrwqof.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2vimnadec.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2inkzrqrb.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2ckipbzwb.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2jwqtyazf.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2yisrmvrq.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2ggpsgvqe.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2movsfath.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2puyyzxdy.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2oqizerje.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2dikrumcp.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2zntowtob.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2lnqjnozl.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2xtdjiajp.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2tmsesktx.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2fcmglwqk.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2nahnctts.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2ffqkqxyi.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2qidirpld.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rvdltqmz.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ymrntmzk.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2ynihhjnb.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ckygbgtr.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2itcdikrn.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2iuyxidzw.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2jqwotjkk.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2wcibwmdr.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2qkerhuae.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2mhdqofzp.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2yuddpzow.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2dhaldrsd.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2xkklmury.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2obazefwh.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2jtlzqvse.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2mnavbinc.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2ezsldyyr.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2rryntuip.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2yizkssob.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vvubymsw.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2lpzybrrk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2rcfqzkmm.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2awdhagan.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2irubjlld.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2iaaqtuwj.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2mygtnygi.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2nrnvxcbd.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2npcltnxh.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2vwhsukdk.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2obdqnksu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mbpncqbp.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2dbrerzyt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nzolzggf.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2oefnotfp.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2zefsiqbe.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2vjfluiyi.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2bjyiizks.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2dmtgyajf.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2huefdspc.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2nlcktzpm.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2wokcclbu.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2ivtguymw.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2ijobpuzl.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2ojfmsfzf.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2jxghmsvq.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2xevkweqy.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2ivgxdmdo.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2jvpwhwxx.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2pzhiqokh.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2eubfvsjq.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2acwqamjc.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2xpmdqdmm.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2nhjhcoob.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2kjigtgpv.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2tfemnikl.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2sceldkpl.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2krjpgfld.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2qhglxhai.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ibrnjnmf.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2ladftsxy.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2fomvranm.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2tpvfdlfg.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2rbqgvzlj.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ucacdnfb.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2btwcppvd.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2jvsmulnz.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2vjgylciq.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2jpiyyfxo.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2eflepjcm.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2zeqbedbj.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2aqxoutsf.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2hmedumdk.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2zzzfwsrc.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2veekitmw.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2vphrtsfy.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2jnmbapio.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2chezxcmw.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2lzrsbywf.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2rqgjfbnx.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2kzregmfy.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2fbfmpmax.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2ufzymqot.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2nfzqkqyf.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2skskmock.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2ixvumiou.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2jdlvluoi.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2gywttmtt.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2pftoadtc.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2yntdenzb.html


<!-- 参考信息 -->