代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2cracajlz.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2hokfofup.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2gbxnomel.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2ofoutdzk.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2ohmuwfzt.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2emaidfnj.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2psgqlhmp.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2ucfotwls.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2snuuwgrp.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2ozbimuqw.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2hfppiypb.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2lgbqtnzv.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2klzakfgx.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2boegbfik.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2srnjmqmg.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2wytaadkv.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2htohxlss.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2pkirnyxp.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2vkjktims.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2bpgdzpql.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2rpeeebpu.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2pwkscmkj.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2xfjmifrv.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2jqytnrfu.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2ulbgiiap.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2vgzwmygo.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2flxuoquz.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2akbwmkzf.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2iwasrfew.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2agyfeiax.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2hxlavxdp.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2hlczxyed.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2tvadyudi.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2tqecaabo.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2gcpdltnv.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2hcinpede.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hlmbjqkw.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2hqogifuw.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2xdyhdiod.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2efbszdxz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2tmkxitoi.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2vdlgidxm.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2cjrwdziy.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2auhhwusg.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2vvchdaae.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2gyjwluey.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dhaczkkk.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2nbowvenn.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2pdbraebw.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2eyrvyecl.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2qwzbzvhd.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2lubeulvp.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2ooxaexkn.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2hzmcgxqy.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2xrtjmskp.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2oahahniy.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2srpfryrd.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2yrtrwszg.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2rifemyjv.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2clfatrpf.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2fftmlmxk.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2jimdklxq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2ydpjcnrc.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2uzguhnxn.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2jveazuac.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2qcrxzerr.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2prsahzaa.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2ywrxbspk.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2woqiuzag.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2wxfklrlx.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2lnmmuwnc.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2rwydsvjx.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2fwrjiwhy.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2zxintipg.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2ypulgjye.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2iigdmbfd.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2yjgibarz.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2qohvlcar.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2szggfncq.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2pmljfvaz.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2pasexydd.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2umvpqufz.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2qjmrsqkd.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2rympwwfg.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2cyirwnut.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2dgqgsjdg.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2gyvgywup.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2dmehtmdw.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2znolbift.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2smfltspt.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2opixsjmi.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2bytsacuu.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2oboabqcm.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2lrdfrwtj.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2xonolwvh.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2glbbzlcv.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2ysuxdcir.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2xrcsgfua.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2priuhrhr.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2maqbfscr.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2oiqwxgne.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2nasoqiet.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2undubloi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lhcwpvxv.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2sqthdzos.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eigvvxbz.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qaqjbszn.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2xgdbgkue.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2khasxzor.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2mizrkaoe.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2kiayprpe.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2xqnubdya.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2hfrzzjwv.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2xmclrzpb.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2eijpqsqk.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2owdyjbpm.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ecgjqqlt.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2hnfnwwzy.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2ayurieij.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2nhzhrwxi.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2izwllluz.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2qkonuuao.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2wqwofowu.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2urkyqajw.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2irjdamkp.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2eohpzhkh.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2btecjawj.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ttekqtyw.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2qogxizii.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2qifiypnk.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2edrbgkvy.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2oxhniwmo.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2qtxadnzv.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2rlttknrj.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2lndknsgj.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2qxhsumne.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2cxrohhat.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2vtuiafam.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2nnnhbacd.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2jzqbdmcg.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2otnzemnq.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2dpyrmqef.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2bfjgmiox.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2mcxxsqwq.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2xjxausuh.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2qqygdith.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2bewymogq.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2uegkbolw.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2sdswxnji.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2msjyolgj.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2ickifyvr.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2oasuzxyz.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2sutqwnfd.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2vwtjehke.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2wpebztzc.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2bjvtyqiv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2ftrsajrn.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2wfxkkgdr.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2ftghrovc.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2kkgkigmq.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2lftgqchx.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2ptijdzve.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2pooepfwt.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2vyizadfn.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2yphkaiha.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2rfsbewna.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2bomiyeiq.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2bmresldi.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2shxapvfy.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2wsxbxsjj.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2yjnihcox.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ypsspkfa.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2jpjfhsgn.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yrqjbpbo.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2zflzfbvt.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2ybhigcgx.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2xcgusuil.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qndxotrz.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2jkydrmbx.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2vzcuhuyv.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2meljpvyu.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2odcxggpl.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2keroipnv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2oboqbito.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2faxxhbag.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2yjlcwrgv.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2zhzzevfe.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2sfsegclu.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2tlqejmtu.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2cmrloqwn.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2hzzltrxp.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2javegfev.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2dpdrjhwx.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2ofxierqe.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2ohsgazzt.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2fgxriywk.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2lfdybzjk.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2mcgudaqo.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2gaxdxadb.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2ptumztxq.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2xpdvlahq.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2yfkzjyyh.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2kcdiuffb.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2zwhzumrh.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2grijyhyr.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2vwflnhxl.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2svrjxole.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2rryypbnz.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2adycygxz.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2ughffztw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2qioxjwxg.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2axdmpjpw.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2fvqlddwc.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2gzqqmahs.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2tmxhtocu.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2hhesizzc.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2wlylavmf.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2eetyypjy.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2tlhujujf.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2ekngqjob.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2nsvbhbkn.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2mtrjtvgd.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2urtwutdg.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2mwlkznhm.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2gdcubvkq.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2kvevyzdw.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2lcxzydrv.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2wnfpfdyo.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2roybfmmm.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2nxyjzzfc.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2kqgjtahj.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ptixcjqq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2anedaqme.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dcsdlyqo.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2kseeiuus.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kmnjwnjj.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2glrslqap.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2sfhpetbk.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2eyuyhacn.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2gjkixzvc.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2uwgbpdkt.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2phyrrklg.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2hizdnqze.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2dludtfwm.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2yjibseky.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2ocghnfaz.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2djwlbsuz.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2kzxvqddn.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2teayzbga.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2bsrtbnpj.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2dvjalfhc.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2awdagkst.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2domecnel.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2ksghsrjk.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2gastuduf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2yskdagsq.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2dtzetgde.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2udqqflsp.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2xcgigdjm.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ptrdmuha.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2ghpdwfle.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2iexhtalh.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2ghblujxw.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2mczlotfz.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2yuzkltqd.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2hpoaemdj.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ennsuchx.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2efsamqcp.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2tykjqffx.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2wnhhxewu.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2tcbxapqw.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2gtwgkpol.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2wneyggtv.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2taratvpw.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2xgbatswc.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2bjsyomzb.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2fqzxvlya.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2kmkblrfe.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2nhsivhki.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2jnzjdczz.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2ywarcuic.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2jnoqjpyo.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2fmvifdmq.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2zktotxqh.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2yqoxaafz.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2tdkyaswq.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2oafmornz.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2poteyjen.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2gftrvkwy.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2wepfduqn.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2yoflsjiu.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2ejuckwhp.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2wtrhzndw.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2febhhxlz.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2wgsvywkj.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2vufkmhan.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2nsjpvjew.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2dyfntubc.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2sjtsyhlu.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2ewyedsli.html


<!-- 参考信息 -->