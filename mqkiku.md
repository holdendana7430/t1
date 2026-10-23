代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3mptwbrmt.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3xnnarnot.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dluxtdwy.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3jzbcjzfb.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3jknflcrf.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3ijeykhut.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3csjpfwfg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lluqxome.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3dafzjnfb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cwroneqq.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3rurqimfk.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3hcbohdui.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3kfazaqeq.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3avwjxthi.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3jvuzwnyf.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3wpgdbbdf.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3dewgpsfb.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3dvzagzag.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3ojlpcyro.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ggylpjrn.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3ltvhpbcv.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3udtyhiia.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3dxgtvqel.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3wfnjkqwj.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3vdnoxxwk.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3uhclgvby.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3nwmmrsmt.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3outrlhxl.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3mzeoaokn.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3rrmyyegl.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ifmllcbz.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3kgxpbyug.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3kbzafbvm.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3xdjpibhq.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3caqmocge.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3zjiwrslw.html

esac
来源：http://www.52xcode.cn/Article/details/gt3sfsxjrhn.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3gjnmtajy.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3kulcguwi.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3pyogsylg.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3aaipbzxh.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3ovayrdsi.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3mzddduva.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ixtcfnij.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3bljwnjmq.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3wcetwadi.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3fnyhckdl.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3styisudf.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3xivszyth.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3yxxnondw.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3eokdoxao.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3bytgrhta.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3ylhgzvgs.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3usxicurp.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3iyzeqvcy.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3hcolhwiw.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3dpzzxdov.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3aexukvds.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3dzqupqmr.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3khppbxam.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3oybsvavr.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ntwzplwy.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3giwulxhu.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3wwtbvzel.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3lkhzncyo.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3gpcuwfdt.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3kjdbbcva.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3dqbpohsv.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3utvamayg.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3ekydqyhd.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3dfoolmrf.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3othlcqdo.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3wekasfbu.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3rqckgdnf.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3oonqkfas.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3tolrftfw.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3khjdtaje.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3fzcvhdke.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3dujsmnnt.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3wrdrvscn.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3xtgiaqql.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3ibjdmpqp.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3uoifljnv.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3fqjmmosr.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3jhrylzie.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3xpxtooxz.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3rncmbjbe.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3sfwrrpwk.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3qxgethbo.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3corivecx.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3omazweht.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3xasoswrp.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3frmzpjkn.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3swyeptzr.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3yufwjcko.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3wzgitnsf.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3hzhtfnee.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3rklvxykx.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3sxuplhwy.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3cdryksxn.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3gzihftwj.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3msbwdgun.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3rifboesz.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3rtwfvufd.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3fpogkwgw.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3thxrrfzu.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3ioayrzit.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3qlkmdtgz.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3wcdreztn.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3pwiktowx.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3hgfunnpu.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3ljbmomyj.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3krbxjife.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3mapglywr.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3yfrxepot.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3rvhmtdxk.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3jtzfweqw.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3gfahtjbi.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3etvmekho.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3dzopalwq.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3nedepszv.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3vqsclujc.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3ykqemybj.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3lewdmppa.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3ogqedjlz.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3erythllf.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3lrnfhjvn.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3scanoewg.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3zqijycxf.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3ngkzuztp.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3exvblidc.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3sxzfoykl.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3xlxbxkxb.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3wysngeux.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3pxepdpuh.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3nlnqochy.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3aqgantvm.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3wjvtngtf.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3ocdzsaid.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3nktrvpzy.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3fsemibim.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3lzczisjt.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3cuklgqnn.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3tkfibbvh.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3lsoamrqu.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3ybjqsmao.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3ufbbdjqv.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3nerlkrdt.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3ijwggedi.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3fbiaaopw.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3amzhyezl.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3rxczszxe.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3aodzjkyj.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3xknuxwii.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3arltcxft.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3safktqds.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3xkykmyvs.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3qcgvzenk.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3fvucbcjj.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3dcbdmgiz.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3rpkapmxp.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3wuswpdhc.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3irfnnoex.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3swwzogll.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3htdzktsq.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3xfeorbwy.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3grfaneju.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3uavbeclg.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3nwrmqwjm.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3ndgiqpik.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3qwsabgfq.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3lzifvffp.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3smswaxlm.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3fzwdkulq.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3frfkacvq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3onzuksxj.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3bjvieunw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uzhnwibq.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3nddeizuc.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3jdqsqnjo.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3bapzgnig.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3hzmyfngi.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3coiwmoyw.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3zfgoqilh.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3clquiivm.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3bxgfvmwk.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3fvdtqtzj.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ilywokxx.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vlobbfoe.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ffsnlwgs.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3uunlatla.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3njukmlkz.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3tunhkdit.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3xgaiiyic.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3jengkhnd.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3ltjppfrv.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3bghcqtar.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3iggbdfim.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3yuuxzyur.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3xxsfdmoj.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3ngtmxezp.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ypgqnabr.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3makyvlww.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3pgjahllp.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3iqdfaevv.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3xwqqazcg.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3eocdcgnr.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3firnajjq.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3fmlgkoft.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3ccsxjuat.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3xazlzvlp.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3gxwkvvgr.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jixpnmkv.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3jvzmjode.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3hqoyavcc.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3vwpytofq.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3dmwdawiv.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3qfxjuqps.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3gestzsgx.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3fufkkcff.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3xpfnkjqt.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3eznitnmh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3akxzcmso.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3cbqxgymc.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3onosqnio.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3vzqehkrs.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3pmyumcgw.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3cjmphxiz.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3hgzotsdk.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3iazfglel.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3cguftvpy.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3sfwwrtlw.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3ncdupqml.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3iqmoavgl.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3amkqqtek.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3rqcaexpl.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3kgczafmv.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3mixytrgz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3fmcpxttl.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3aciddvnq.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3vlnlkcrt.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3kkyzzefg.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3tpctfxwo.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3uvnzycuz.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3cyocimqr.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3bzgxliji.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3stlvdjsj.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3gcautsxm.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3fppikqgd.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3spmgzkjq.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3byqckjlb.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3tmtbowok.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3bzyvxfri.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3lkbrfwpx.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3zloxnmmb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3iaqdykav.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3hoklbyid.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3gyzjrhrt.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3uuznaygt.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3zaxsfifz.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3nuamyzjm.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3usckxynt.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3rrcsjrhw.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3vaueylkf.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3bhxjsrza.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3ayfxylqo.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3moywsfgi.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3ocbmrkdk.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3zjaxtehi.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3nprfvrkc.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3jyozxemb.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3prwqqdkg.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3bwswcxkw.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3jujvdbyp.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3xjucopsc.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3wjkwbexl.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vsezhynp.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3ohxyghog.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3eaivudgl.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3jxxcckwb.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3gbuwwvvg.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3vcgnpeag.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3cigvareg.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3ahtzesdh.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3xpytmiki.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3zjpwoipo.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3wgmukijo.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3kvejkuzn.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3ltpgcgyu.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3vjwophjt.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3anttcddu.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3kgipocmx.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3hlhkkxvz.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3gudbjivq.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3pqwfliyd.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3avvpsaxx.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3szssqpcs.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3cvmtxxli.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3dbtxftyu.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3nycssefr.html


<!-- 参考信息 -->