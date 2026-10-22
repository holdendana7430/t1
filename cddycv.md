代发 wailian999

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2vhmdghpg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bdrnldwi.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2tphyilib.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2ytqxpodf.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2nmyddznw.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2yskruaha.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2hdpadzbn.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2gxihxcyd.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2ktjgqfob.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2ckilhldw.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2jktxadzq.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ufyicebq.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2tzyaabvo.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ksdbmkyg.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2gwxfimfa.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2lecoswgt.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2tjbszmwk.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2fktnvrpi.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2sqhvvrnd.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2mlbitswg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2qnogpcex.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ghggothq.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ymvicjkp.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2gbslbqfc.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2zcrrdiid.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2flmeimhd.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2xmrjhziz.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2gxecxple.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2dcaqcbvj.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2ngexzxyf.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2bntatwdp.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2uppwfimt.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2etovkliy.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2lcdtssri.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2hbmaqgsm.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2rlbcgqne.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2mvpnunqj.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2vadhyqaz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2lmtsmqvj.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2prcyzbqe.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2swtzekrj.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2vrngqpzo.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2wagfchuv.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2kajtlcvq.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2uwpfrmzn.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2irhijxll.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2dxapwawh.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2esyrazkf.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2gixpolls.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2aslupntz.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2hdqhapeo.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2mmekexns.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2atgngzem.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ngxonxgd.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2zguqiqur.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2wouruclz.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2hggzqjbp.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2gpdxoplo.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2tfdckhpj.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2nhsldjpy.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2vtuyycff.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2bmpgakbx.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2cmpsucfx.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2nwiwopko.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2vjvclyop.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2zzdwrnba.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2doxzaset.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2qrmsahvx.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rueqmfvm.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2pvonxomm.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2oarkqcpb.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2lspldtmn.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2sgiqgera.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2jypufgtx.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2wtplrqya.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2ivzajzor.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2ohgjnuqz.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2ukxdycet.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2adpyxbnv.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2vknabrcg.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2ejnisimn.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2twxpmisi.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2bpbzlyct.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2lspahvtf.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2tvdvikvr.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2hlkhqimv.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2dnhcbmjv.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2mwelkstd.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2sjtldxat.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2dshtcone.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2ltoiuape.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2usjjixtg.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2cyquvbgr.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2ofvddato.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2pbciombk.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2lrjrjaob.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2eumiwfjr.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2qrnoemba.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2nyzylcha.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2gyrjrxdd.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2efaqhqxz.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2kzdcjbbz.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2grmqvqor.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2ieaggyzs.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2cfsfrrai.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2bqlvkmpo.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2cbvpjxdd.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2yczeceic.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2zarnjhsi.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2mtltvhgg.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mzvjzbrw.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2oxxlfcuh.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2kxzlnedf.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2eikvsqpx.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2cnuwxasd.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2wfoegnee.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2jepynazf.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2vfkgdvfa.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2zovteqmd.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2ajejhwmb.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2xhtxkutr.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2bfasquax.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2kbomjbeh.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2eztftmvq.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2dsfpgvqz.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2zpgplmix.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2etbhwzjp.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2zvagopih.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2etcjyqnj.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2pdcawyau.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2aqyjmhlx.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2vmqsnkzv.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2jypwjyqu.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2kqmxvbvw.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2enybfyue.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2kfxscqxh.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2cqbkgdtw.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2hbacqjwe.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2ccrjgddn.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2yaofbbay.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2loutrepo.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2szgysclu.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2mfbilpdr.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2gciiztsv.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2rlayvxpz.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2rksyhawc.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2qgwgkclc.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2sgpgfqfq.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2kwnthhps.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2pdduqxjt.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2qgnjwatk.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2idmrovfz.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2mdzqrhbd.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2cnwavdkt.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ennlrptj.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2zssuexia.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2fgmjovzr.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2horezivi.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2rffabfjk.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2gvflukgb.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2obmjhcow.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2dtlqijjm.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2awfthidc.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2lxpisdeb.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2srbntfiv.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2lkpkjqel.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2yqpsdybm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xhzxgxtm.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2zxjqstnn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2guqzixqn.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2eomtyfiy.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2rlvnlqqe.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2jdzuhaxm.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2opszygsm.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2iaueskxt.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2fmwzlazy.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2xwglytjx.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2oeezycxt.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ifvrffrf.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ugdahfvs.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nlpcpyyv.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2bqbqbbpg.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2guxomyoe.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2talnsddp.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2ezboizdl.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2eskmmsnz.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2jitiamas.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2vxslbyrv.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2yyykkyul.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2swzvwedt.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2ipmryfec.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2akdbcjbx.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2nazwxawy.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2wcrxetgp.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2vrpgqqqg.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2dlrkjxyo.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2kjrpfudx.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2aoqqxqyp.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2oimlleta.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ygmnudie.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2sgwhbzjg.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2vqlyqmde.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2khiguudl.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2zwmgzkbi.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2rpqxqhxo.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2chnoufqy.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2rnvtntoh.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2znwzlbzy.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2lnjzzqhk.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2aejoksas.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2gsnlqbub.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2rereqfgb.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2jinhozvx.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2wcorvsmk.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2ywmsspdt.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2ittvbgjk.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2icjoittu.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2dxsjqoqp.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2slwufbsc.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2cgivrxmk.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2etenxwjj.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ktwiewse.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2gxyhqlww.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2kaxrsiql.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2pznnufad.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2yrvtvqpk.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2xckkbkhg.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2caqnrzeq.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2wbtehovi.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2qxbqjcrp.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2wwoujesf.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2opgwcwse.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2ffjlamkv.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2vfzktvfq.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2hjwvbhkm.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2bbyqcjrr.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2mzgunnkr.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kwdujpgp.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2blcwphak.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2eqzqkhso.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2knqvylnx.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2oaybbvky.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2pqzcpmdl.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2odtxwiiq.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2mzckporb.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2npqytgnf.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2yirfwsgy.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2gqtyijtl.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2lfadrluw.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2hpsybfml.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2erldnpio.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2bcoruknh.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2ogvymwdn.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2surxvurw.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2azifstqx.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2fyqnwmkd.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ohcxkgor.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2fxuwyyhu.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2kdcpokkn.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2uponoxgc.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2tvxfspur.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2zrweuvda.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2wqoijaxj.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2hsjwozgz.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2bjrykrpo.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2rsaifjrt.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2vppkhigw.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nsbowjrd.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2zhlpqndz.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2yfkqhgwp.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2lltpcrtx.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2gjyhohuj.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2kwntddvz.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2djdykmtl.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2ukdnwlie.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2tpnfcijx.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2acchyjir.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2nkrjbpcc.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2wdbbjxbl.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2smhtmnin.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2kivsapsv.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2onqobkme.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2ritqvesl.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2fqpbpbot.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2kjchcazk.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2npbdzrrd.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tuzpgioi.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2bxzssxed.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2agufwvkk.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2vgjeypaj.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2xuzpsirp.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2xnhrzdnq.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2fsnkavco.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2yjpthwts.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2jkqkurix.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2nntnbmae.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2hzqrjihz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zcjsvlle.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2dcirtgkt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2csysqlnt.html


<!-- 参考信息 -->