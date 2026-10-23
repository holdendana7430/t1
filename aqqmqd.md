代发 wailian999

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3bwwmpaeg.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3lgzyqfmu.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3qqgxmhrt.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3ijblzuyn.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3gspmcsrn.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3kwpjmapn.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3aqudosdz.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3mmgolrfy.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3akcpxsse.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ashlvysh.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3qjjmcjzv.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3sjrwdrft.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3ekjaweob.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3bnpsnmbt.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3lbpinrtw.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3imdojwre.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3mrqdoikg.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3ozbfafdl.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3ohnffcti.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3xxpviole.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3gtsrghkd.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3hvmexbny.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3dvwdjqnn.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3dckosaam.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3houkwuoc.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3gymsmuuk.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3wwaxdede.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3xwfztwwt.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3jaxavwqf.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3zhaspdzt.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3krzlszyc.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3hrguhoam.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3neqshrbp.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3leftyibl.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3cytaqbdr.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3bajmtqqv.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3hedayikf.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3jrcurmha.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3xfumkjsu.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3utfuovto.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3nnatfwbb.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3xnojfxyp.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3duwfjije.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3jbjibqfe.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3cadlvuzd.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3ngnchtmt.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3hicwjmak.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3yctuajde.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3xsapmpkr.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3zsfluxtc.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3ddgeauqd.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3whbctytk.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3yfoslnhn.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3zwcydhry.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3miiqylup.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3yunzdtvs.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3rylpuapb.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3ovvotmmz.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ufflphsv.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3kgcniaxa.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3pblrzdbr.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3jhdrnyih.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lvvxlqqr.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3zumstntx.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3hgsvidwd.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3nlmvlcsx.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tcpufoki.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3gkfcukqj.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3kdzdgprj.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3ujzghrln.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3xofgrhcu.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3rsadnjkd.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3srpngcmv.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3wowmwfjt.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3hshsdqud.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3qmwxxbsx.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3cyxdcysu.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3zdiolvgi.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3twbesayv.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3ggguhesd.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3yjynroog.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3bcrmrdqg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3ostidhzm.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3feedoabl.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3pphxfpty.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3kqinvxlt.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3xgvlaatu.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3qsmugpms.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3kgkczjvx.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3jhellktz.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3ggocckju.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3dynfkgvj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3eyslmrzv.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3vbxhahkg.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3zengmrpk.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3ucpxpbww.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3qmvqhzbt.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3mvboijlj.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3yrantuul.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3xnqvixse.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3rwxvaoil.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3okpcqzke.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3dndefvxw.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3kzyqorqi.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3dcozsmuj.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3ftttvgov.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3ytnxgled.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3wabdvvrc.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3pztgxpwb.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3jljhmukt.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3gvmhfuri.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3khmnbqrr.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3mmvgmigs.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3xfecrppc.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3hvslbjxj.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3hodvhqez.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3fuotaola.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3saprrgnk.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3tdzwljdp.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3iyiebjeq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3mokldtyb.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3gbfjjpoh.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3mbbyaned.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yknmodbz.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3brfkxyeo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nxricxnp.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ygfwrzme.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3xykpqumk.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3zmsyctye.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3gnqemuyu.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3byyqbrqn.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3ihhrgbwg.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3iypbyouk.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3ttzvmlni.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3zvkmcxbx.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3lklalzep.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3mbzvfget.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3sttiiuga.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3gxdwtdzo.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3vlpkjtfj.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3uzgeqdjq.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3aptdhceo.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3jylquwqt.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3kmvpwhjm.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3yzvskgtz.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3rbtkoruv.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3tcngygxy.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3cjsvdiig.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3xoayfiuc.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3mpxslzvq.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ugrbqlwl.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3icnmtwtc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3nzsnzwlv.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3zrcohqfr.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3ibrmeuci.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3hdzcvrnw.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3qcuunilm.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3dudkyfzd.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3cviyfvru.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3iaojeufy.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3wtukiowj.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3rtxpbfgo.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3rgrbjshw.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3znrjwibp.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3zugddorh.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3yhitgash.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3dwlfizqz.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3cowmplkt.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3xluzvdem.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3tmhhtpdy.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3hvqmzbfq.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3lqzojuba.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3jshbfoyb.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3aehyiplb.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3odmqprmb.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3bcuyvaec.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3hbzoadmc.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3izoluisc.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3zfknkatp.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3pevfusrf.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3debaylyp.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3ljcvatlk.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3zjicbjtl.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3ifvfteqz.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3opwqtsdt.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3qbvztfzx.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3knastbvz.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3tinlwasy.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3qjqupcvi.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3auqdqnxb.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3zjahsago.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3dzcnmcku.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3ojwhwwjo.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mslyxqwu.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3oolxzfuc.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3rkigvsko.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3zvfwtezw.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3hnpetspa.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3dnpthvlv.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3bmunpoox.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3jvcxyhzl.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3hmsxoqnx.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3lzfiyitv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3nnlvwfuv.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3vvzoejyy.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3zxppgitl.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3hfxrxfuh.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3jdntmude.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3tmozueje.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3avwcznbf.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3kdbhfifo.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3xyurbswl.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3joamndso.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3azzrxveq.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3lcnhshlt.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3oqlwlhje.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3mhclzvvn.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3dpnjjnui.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3rhqzufdl.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ulnyugwo.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3mqrdbqyx.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3mgdzjuvw.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3gsezrmse.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3cgfrrcqv.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3wftajawf.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3zlmpvgfy.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3kthznjsp.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3ozarsxlg.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3sugfxjzc.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3xwxzrthc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3htyplpts.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3lrjfuhnr.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3mrqfcpnw.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3kolykylg.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3kfngpruy.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3zlxtacgl.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3dfxztnvx.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3wxaykvsr.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3ndmukoad.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3qjkgefzw.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3kzyhjdeo.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3xfqwkauv.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3tcdfnabu.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3tqntndij.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3vtaefmqd.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3tmulbbaf.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3rxdcyehm.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3qrhjwtxa.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3vsswyows.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3ltozsept.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3louxsija.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3mkjalmgf.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3rdnjxyyl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gfqylmhw.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3eehnfijy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3empxbjtl.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ujxwjuzx.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3kmkrvlhj.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3vmidzilo.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3pzgsuqcy.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3vclmsnye.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3uoflzcmj.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3rbetpccy.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3nzmzybef.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3atwmyobg.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3llindvzv.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3vlmvvddx.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3zrdihahy.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3btopoqej.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3sfomwwju.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3jmjbdmhm.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3vqkcdety.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3scyvwhua.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3qmbwkyjo.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3eosdhjrc.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3bkjdxrnj.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3koleagmg.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3gujuvvbv.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3mrxoumxu.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vtxfztrd.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3zeabilet.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3luaaekct.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3actplnra.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3qdotoqfl.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3pydzkwyx.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3bhmmxhhl.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3dlckpwli.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3aufflrqw.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3gmivmkag.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3gqayvuqq.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3jnqkedxi.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3pwszmlfx.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3tmhnjhrm.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3hbfaplai.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3jrkiitik.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3svngmbkj.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3oopgkqjf.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3ovqknzze.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3vjunross.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3jxawmzpb.html


<!-- 参考信息 -->