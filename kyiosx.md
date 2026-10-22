代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ibcquhot.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2wnxsdnmy.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2jkceabra.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2fgvdisum.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2avbqyjex.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2lznbhmwh.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2vpzphajl.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2uqhkskkh.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2psdoivsf.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2gdtlwvtl.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2wjpymien.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2jzenjtgs.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2jswtwoif.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2uhjvcnnt.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2hqskkvsw.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2ogsdlaan.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2kfwhmysm.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2kiqmaooe.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2ymtomilt.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ltqwlkhm.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jzsxtraw.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2otrxfrwp.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2nxcmuzkv.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2pewieifx.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2achgepsj.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2kiqtxmxu.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2vlsbcvhq.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2fmaklppg.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2baktttwk.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2tugutxru.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2xhbasojp.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2losyrlvv.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2zifykpuy.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2imntznuy.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2jqgimsqi.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2qrrpaapg.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2tshfutcl.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2tmjggxgq.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2pyagdavo.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2kgymswws.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2eakenyqk.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2luupxafl.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2ovuxmykb.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2uwmphvcc.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2ziptunsm.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2loytamuq.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2rksqzewq.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2rvoqarun.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2fliknvwr.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2yilunizs.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2jtxhwvfr.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2sevfjkpd.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ulxzgqme.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2oizlnvcp.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2aaxvaryv.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2siorlmmi.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2snqksslm.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2yvjbciul.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2gqvsadai.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2lsqrfkag.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2razgfglr.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2mmclekda.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2yqmnjfdt.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2lcdwfbxn.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2clygryrt.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2vpdefuwc.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2uavjawnf.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2tdfxpecb.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2sjdjispv.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2tscvjkul.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2tkdyvcsk.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2kqqlhztk.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2rpckfzfj.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2kqgmojfp.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2gtdpgjne.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2tewqpaoz.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2olyrvcbc.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2cdplmgsj.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ygutxqyw.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2zylednmo.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2dooeryob.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2nnwudjoy.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2ayjmbbib.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2opjjjerd.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2rqiqzwfm.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2wehqybem.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2mindqtto.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2tvsmyhda.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2ucabyqnl.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2ciqsvlbc.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2vhmfyxru.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2ufoizamj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2xeadtrge.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2efwjdvcz.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2kienxazv.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2bkyikcdk.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2pxocdvmo.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ezqpprrc.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dnngyqip.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2npfohcvs.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2adtkbwwp.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2fxknwpeg.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2jxznjgtt.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2agsjfnle.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2wilwskfh.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2unbkstty.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2dwwxyhdt.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2gftzbsie.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2unpdwahz.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2gxwlrcuj.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2ulkenycq.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2bmwprzmp.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2gjxizcrz.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2peeedqdz.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2xvaosfnb.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2hhxbqdzq.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2gishgjup.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2mxyhuazq.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2tirpnowf.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2asjyxwdr.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2hwolqfqp.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2cticnzut.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2zjabchgb.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2bzjpojlf.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2tmfmwxvr.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2afjruppr.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2dlrbuult.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2itixziam.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2ogsofinp.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2axqkvpuy.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2gmwbujeu.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2fgwpbnvc.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2jyrkgxei.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2senfrniv.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2nbizekmx.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2hnydklcg.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2srpynuyd.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2vygtmzlh.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ytgchppn.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2lqxazgym.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2mzctsjax.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2oabedlbl.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2gmjzeffl.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2uopwryfd.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2prwzjnmm.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2fpibccdy.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2sidzdcng.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2bbzoezxu.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2matdukhz.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2bckjufbj.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2nymxkads.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hptxwdhl.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2ndgzgrqz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kdajsiyd.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2bmmzpnna.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2esglkcls.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2plbsxzku.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2gqpziufz.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2zzldinqw.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2nrklxhuu.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2gfmvhzpa.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2pkzgxocp.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2hjsrkcjn.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2elrzzimx.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2aqzoirlp.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2hadwjglo.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2zilmgwkn.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2nbpggckq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2khyqgyzi.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2padjickc.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2ebnpivnb.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2ufgxyudi.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2egzbkkoj.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2ulvrizza.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2fumcocnw.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2sezwxyys.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2vrjkaqld.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2kbhociqv.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2vvdmslnt.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2gacmlfjd.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2wmhzndha.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2zfhuweko.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2hszevtrm.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2jzwiensr.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2qaymvfkp.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2fkjvhsga.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2xuhtdejr.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2dotwuguo.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2cujovnzo.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nfllqlpo.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2joweyonx.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2jxfnrmcc.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2xscyiqof.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2xcwwyfwp.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2gogettzl.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2uolngqjc.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ayumowrn.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2skcajlvs.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2yumnizso.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2ujmscyil.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2fzvcdchb.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2fxlyztuc.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2qdssdlgw.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2dihfiqjd.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2lbnwumlv.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ksictlti.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2dcvrghnr.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2xcleypsi.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2eypzdegh.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2hhsnzdny.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2tdqqfmfx.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2clvrurpw.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2dgqclenc.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2yxhluytw.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2smoqdmah.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2kjamfahx.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2vcytftfn.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2bcgvwfzk.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2ehwzjiaq.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2nnzgtbte.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2ckyyhwpj.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sdlzuskj.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2easnszgw.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2deelodpe.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2zmdbwprm.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2kzxqmbqf.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2rswwgeiw.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2tvzwopfm.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2biucbnvo.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qizsqqex.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2frbazevn.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2nkqurtsi.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2cmgjfhnh.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2minwhoej.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2zhvvlrfv.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2dzdmnzba.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2ekasuipv.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2ockwrehe.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2njnjnads.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2wbkidrvh.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2ppefyazt.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2pshrybct.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2hcnzaiia.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2metuvhcp.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2ixbzjfon.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2svavydtl.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2yaiwmupb.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2eewuwpcp.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2zxbysvtk.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2nvjvysct.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2qqggpegk.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pgkbuhxs.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2pgbixdat.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2qzddfbhz.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2avpigzkg.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2ghgaysek.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2kvxhnrrl.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2rddatuxx.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2dhlwqrus.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2vwvpzbhb.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ticewxld.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2mlgghutn.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2hbszcedr.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2lyzokzcx.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2poyekdht.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2qnpzfysz.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2jtofqqhx.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2mmjdfsuz.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2anceivcb.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2vucaocjc.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vdnypdci.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2ethwbixd.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2vqjcldxg.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2jwvxruko.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2lctqmobs.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2ceiurrca.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2fenroxic.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2bhquyyfv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2azdbxgzc.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2bwzvuubf.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2sykqodqb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dvaeuqwh.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2ixvmlqav.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2epxxetop.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zwhvzcyd.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2lwlyjgly.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2nofhzcsj.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2weshplou.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2bmivkyjh.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2comgjfjf.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2puljejrk.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2vtcsvoig.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2roojtqbt.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2vxyazusz.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2khvonens.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ztzubfda.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2wisjhelh.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2yslqftuz.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2hsfumefn.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2cbvimjnq.html


<!-- 参考信息 -->