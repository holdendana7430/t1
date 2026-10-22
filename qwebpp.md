代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2gtmjdvmd.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2duznpyks.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2hiqkmfno.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2kcacgmvo.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2jblpkmnu.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2ojztpktl.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2fastlwzx.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2jtsfmtuy.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2ihaqiynw.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2qlsfbmvl.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2gatkflrg.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2vaiyaedz.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2nymyaqsd.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2tvdrijhd.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2goooapmm.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2fuscopiz.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2esvcnkjp.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2afigbjqi.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2wilsudma.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2yplylege.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2zfqidlme.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2iftvdwjd.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2legsopki.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2hgzkezti.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2jfixvsog.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2rwfbxuvg.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2joegxabl.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2cdfpgacq.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mizbvobw.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2zidzgxwd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ammwsawr.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2xezoyssw.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2rkwwafrk.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2aexqdaox.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2pwqsrsxm.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2yjnvigkz.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2dppxohgl.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2jcgchlea.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2ehruxzvw.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2wpmpiwwo.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2eabnixjb.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2fmybeohv.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2ltlevwde.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2bvatnjip.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2jrfjkewm.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2pqwisfcs.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2pnqksngn.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2npahobxo.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2eqlrjyit.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2qljhuuww.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2sefvjhop.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2gvxkvcdr.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2mzgrgzbj.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2dvhwtuzf.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2zoznqyog.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2rlnieytp.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2insebjvs.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2tmsuhfft.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2hncvtage.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2hkavblte.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2qqpodwvi.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2gpapmwqt.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2lwxyaels.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2eghtbgij.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2ciwlzqvw.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2avzdoftr.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2nugakttn.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2leiowjhs.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2hbnkbnxn.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2ipbvmaqf.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2aashfudw.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2wcstyvsr.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2hrdmnjdz.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2rgoxrfud.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2abmlnnee.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2ivjbnwij.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2grehvulj.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2dumwrpla.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2wzwtbrds.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2srfeoihy.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2hxtdgfyx.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2lwuouyvj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2tduokfmu.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2ddridslf.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2zpahgvon.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2djfivgiu.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2eessllle.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2aoihacwn.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2paawpkiv.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2vhvxceyr.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2kklwngjh.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2adjqhxfu.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2dqyowrym.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2zjhrfliw.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2ocgqivbn.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2zoulylij.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2nbuiynxf.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2wgfupfmr.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2avfyczav.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2uogntxyw.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2dfowpsui.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2idwtzbse.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2zeerhoyr.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2brnmxbcu.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2jgidmshn.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2lvqeofmb.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2bemtsaip.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2hzeyuvmp.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2jaiqtzpw.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2nrphykxk.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2hzulmawn.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2bxbkmimk.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2lramgrac.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2mjbtlqlh.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2bakqizuc.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2zovxojww.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2kmfkykwn.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2orimxgyl.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2iffhbmmw.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2amvupbin.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2oguohjwp.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2cjublobb.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2onpgoqly.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2sncwrpzj.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2hzfnizmi.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2wqlosxfq.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2brsltxep.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fbmtsxts.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2rteahdfa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jdcssjyp.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2asxdyiie.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2gidjmuzr.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2zfisiigo.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2fmbwmfry.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2uzxgvqyo.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2nkrycqnz.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2tpsfeznu.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2jqrqybxv.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2diwaoywg.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2qpcvrirt.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2isrslmqi.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2tcoutvdf.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2ggdrclyb.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2oqwtlbzd.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2cnmceywj.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2xjlttmxa.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2qdvwrqae.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2fglvuelv.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2aswswlnj.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2uykexqdv.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2wgosxuth.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2psjtbndc.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2zsfzciim.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2qrtjfmes.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2gjdjsqgv.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2suammprc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2atglphal.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2hdskptdj.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2uaqxdodb.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2eudiohlp.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2zrddeecq.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2maniytoa.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2kiwwkcfv.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2wddenlhb.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2usetnevo.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qwooppsc.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2zfpsqaoe.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2wfvezdia.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2ljvkneny.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2lwerztsu.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2dnwmqdfy.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2bmdhqaat.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2kaywwnnu.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2pwymtgey.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2hgcaelzh.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2qswmwauy.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2gbumlfkw.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2scailwoq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2nbayzsnf.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2emiuvhki.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2jmoxzgln.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2oixeulzp.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2mjcakdcq.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2tvpayiwc.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2idivrvcg.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2nspisgzy.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2vfpfamoh.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2nxlcrokv.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2dyghmyoi.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2cmxbtucc.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2txitmtnz.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2wfismtba.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2wocfdcjy.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2gspvegae.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2juwutbvx.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jmqbjlxd.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2ijreyfif.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2repavamb.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zhcdgkdn.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2rkatjtwp.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2kczxirvv.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2rziavsoi.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2jdgfqtzj.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ghbahhjy.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2pgybleve.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2smqrpplm.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2rkkvctoe.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2qftuiarj.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2qgpmgkol.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ssscvnmq.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2viwyemjf.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2idfdgttv.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2vgauoxtn.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2gofbtczj.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2utuioxkc.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pffdhjbi.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2twnymvsy.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2zkcvhlxs.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2yglqdknw.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2nvqpezqf.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2ggfgvynt.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2ibalebyf.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2zdawqtxz.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2scfalmqc.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2dkxiuguw.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2bpjscsus.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2nhfakrzc.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2wwtufysw.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2pljozeyp.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2etjbusiv.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2bclmhskt.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2vysbvxvv.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2flnypqmr.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2kswylukd.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2najhgmyw.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2njlnlyuy.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2gxqqaaij.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2bbaaldsg.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2fiwpbefa.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2zvybnwhg.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2bkdjfqsr.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2oeloanmu.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2henbenye.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2qkzzcfnr.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2kfdwdbhs.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2oizcsxvc.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wjzikoit.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2qjuabnlg.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2kfazpmgk.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2hendeejt.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2ihnevdne.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2hajveklc.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2gjnueihv.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2itbslvxp.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2dczcsixk.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2vglrdwin.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2tahjpjqd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cohryymz.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2wxiotoyj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lercomyb.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wenjqczd.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2nnhdbbhg.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2gvcnxrkc.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2ttkwbnuf.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2qeyvgtwn.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2ysyulgbo.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2yzxxjqmg.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2rtuktyzp.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2hlehkgkl.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2gsulghhs.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2mnuvzovp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2rdjusqtw.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2vggmxtig.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2rgbdpbzg.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2utcaswcs.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2gaheczal.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2ataddwct.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2rbehezjh.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2omnsugok.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2nlerucom.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2asiyjvvh.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2ipcprwng.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2vobejxvt.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2blhwydck.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2qwuurtuq.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2egfsmprq.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2hmlbqdqz.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2puaqnuqp.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2duzhkfum.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2maeleubl.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2pojjcdiw.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2bzrbtagn.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2qenkcauw.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2jekonslj.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2cytioobm.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2laaveoka.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2agbnxwxq.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2ckpftjtj.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2qgbqkouh.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2xsorzpre.html


<!-- 参考信息 -->