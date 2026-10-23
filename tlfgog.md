代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3hrnwzkse.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3suefzsjk.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3evhogmwn.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3opghbswx.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3eigxcfrc.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3sggniycm.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3gvadbqbq.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3jdotgsou.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3xzwvbvkw.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3vbgvkbxt.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3vjfcywtq.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3mthheqfj.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xqhrdjxe.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3saqnnvwz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3hkrlirnm.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3deychxyt.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3dwltpast.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3telhepzt.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3sdduarep.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3wipelidt.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3cpsofxic.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3ubdldisc.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3dnxykkqo.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3ydskllxl.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3vfmhnzil.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3vgdecqqe.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3pthdhilv.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3onwopund.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3qrohnatx.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3trvwfmio.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3jxldvzgj.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3ejzdrcat.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3atycuxni.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3iavgdczl.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3qmcjspkx.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3kkafpbxm.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3rrqiseqr.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3vkoipmeb.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3qjjxhaou.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3wscfokbp.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3pkeubvil.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3hjnopkco.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3hjchmdkv.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3orqzolpz.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3hhsfxnfm.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3kijmuecw.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fuzeodli.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3bddfwget.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3purfunwj.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3ertflycs.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3iypniaqp.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3aqeffxxl.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3uvcfjbab.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3ncnhiknk.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3ctsddegl.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3xvcwranp.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3ktvhbnct.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3cenkbinz.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3ffjeghxw.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3tceqznss.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3iaoqyvga.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3whxdkmbe.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3wpgsligx.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3ctozyprw.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3rpvrqqxq.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3olwpwhtv.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3judmxrce.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3rqpbjeyj.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3asvaiswx.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3kahtafqc.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3hymenqaf.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3nnozwyob.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3zzbpzmzs.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3apldyfgb.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3widzazkp.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3lcjthnyt.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3zmxbqmkx.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3mmrybreq.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3hszrovgt.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3maonzfeb.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3ycfsexmr.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3yzzzckbj.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3ktkjwhgi.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3mnjomntc.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3xusghdoi.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3rdamjmdc.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3hjivooqj.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3kcvozmyu.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3mlfzcryy.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3dynqhtst.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3lzdudmfp.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3zdvyaawz.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3mmzwmaab.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3fndkzwtt.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3ykkouoeo.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3ghdudjjh.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3wmlstvud.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3xbcrnwtx.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3hhjoycke.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ncgpmbtm.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3jbenvifj.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3zbldhddd.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3cjkqawgn.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3kgagjogy.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3jvemqtrv.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3vsusxtcu.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3incnwqdh.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3ckhoposh.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3jlnolrio.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3nhqaxsyg.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3qyfniydp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3isfxfzsl.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3yefpjrnb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jiqsmywl.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3aidcqcyx.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3rsubwwna.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3tcfvxpdj.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3fciumrfd.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3hinbnfeg.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3efeunjrs.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3jztheckf.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3fnamafpn.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3raysddqh.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3clhuqevn.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3zwspyqjy.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3gshptbon.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3kzefmpby.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3pwfgljxu.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3miyrigja.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3gzokwikg.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3xlkzwtzi.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3dipxuarq.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3ubwsvwqp.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3sdsmolem.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3ajmlyyxb.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3owlitxqh.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3yhesncss.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3kgbglumj.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3ghoynodl.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3iscwdzbp.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3qkygcwhx.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3fifekfjd.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3fbpryahy.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3dkjfldsr.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3fdpclsqb.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3dkoxavox.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3canjiocr.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3bowjyzxo.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3zxrbqdkf.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rjsrvlqv.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3izggfacx.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3xutnwrod.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3ovsbbgyg.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3focidfoq.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3bmyonyzk.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3tftztfyg.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3lhcucqro.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3mfaxyqpf.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3ipojcznr.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3itcfzsec.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3korrqtcf.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3fjebxnra.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3fslhbxpf.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3yzndcsao.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3ovfbnzer.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3gqjihhht.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3blgiqpyn.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3jxtgxevz.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3rigioyrt.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3petdlvgl.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3nuxmyzhz.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3jstcwsqm.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3cwxlmgkk.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3hkvefbpp.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3kwcyqtad.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3vowlepiv.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3mlmgrxtw.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3dhiylekd.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3srpazyub.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dcmohxsu.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3pqhlnjeq.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tcgayspi.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wimynmhp.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3qfgbgtbp.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3hiegooyp.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3vlhluvht.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3luvrqons.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3aassmloa.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3ajeitqcc.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3zejlluob.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3yzfxluvd.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3dlnnnnmv.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3mwjeajxt.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3ifmzolwe.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3nqtnmpal.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ewjzmqcj.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3cyulhkhf.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3nafkbaid.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3yflmnwbg.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qrbalrkv.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3vvjnnawh.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3eabnoscj.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3ssgpifnn.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3kvyjquli.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3rarzzpmh.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3fxjsavxf.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3snpkquqf.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3ovattchq.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3dozsktyh.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3uzpslavo.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3fkyhxlmq.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dbroyung.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3dmubswdq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3nxotzkzh.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3wcdqtcvj.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3iiyvsntb.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3waiskmow.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3zmdilukv.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3adxpqxis.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3psbjedru.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3fyqirznz.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3slbdezjs.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3ndsmzlww.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3kvjsdqbs.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3owafirod.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3cjdzkidm.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3qrhtmezj.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3hfizbkty.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3wfwnyihs.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3pmvqvozc.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3vvlpbyxb.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3ftcpmkpm.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3awyuakri.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3shrcuuem.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3vgqotxxj.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3clrlcuyy.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3efklzpni.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3nggrqiqq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3hjkobien.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3duyupddl.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3fbhhrkdw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fphpzbok.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3sikaomxv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3myubahlc.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3riembcwe.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3bmqxcrel.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3cmrsosxs.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3qspjxctl.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3lqisqhjh.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3manxxmzo.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3uyhttlfj.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3ddgblofy.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3ydyazpkp.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3rvcrnxlf.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3ufowahep.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3xqkfthgw.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3stickfdm.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3frrtxzwt.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3suoyysbd.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3asxedenb.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3jhakxmft.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3cbbnbnuj.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3zmzgriwo.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3pohhatkt.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3twyfwdqw.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3bdcxwwmy.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3bhxwqgpw.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3sibotzte.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3bkrnwlna.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3vvsgkymc.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3ceoijrqv.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ckzhpuhb.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3axaivjgp.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3blboiruh.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ktpyblnz.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3qvemwkmp.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3yofhxktb.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3mkiusfxe.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3rrkavinq.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3quqxluid.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3laakoafh.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3xbvhcmqm.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3tjlmxsbp.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3xeulrzjc.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3gipgirog.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3vknfkksr.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3prnsmjxy.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3jienigrc.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3lfscucis.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3zsduqfic.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3gekqydfk.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3sxrjwwyo.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3oxbijjbw.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3alrtyuwk.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3khilytvy.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3foegbwaf.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3eaxcbsok.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3waulyetc.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3dpcjonvz.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3zftzwuht.html


<!-- 参考信息 -->