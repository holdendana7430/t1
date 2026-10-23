代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3kvbqktub.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3dhgqdeyw.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cfngayqm.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3xgqxmvkz.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3dmhkncqu.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3senkfbxx.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3bxumgfdv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dnrsnrkn.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3mrkagjzu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xlhizqhk.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3bmflrusu.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3osatxkmh.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3kvxeqrrc.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3rbmgnhbp.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3dtcicaaf.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3rkubxtvk.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3arwmxvgg.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3yiutbidb.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3qcmhgzpx.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ghrtwrut.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3fnkjilee.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3yexknbkb.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3zclvcenm.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3ejzdaxkg.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3mmfsdpvy.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3xoekztuf.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3jfidxvhd.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3bvgtcwjo.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3lsfdljjd.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3kzjnldfo.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3hampfics.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3kopodjgd.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3zszobktg.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3phgecfil.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3ajqusfmg.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3kwntdsir.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3tlivfiay.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3uvnbxylg.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ascahyhd.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3wepylmzg.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3nzoihbhk.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3hbiqiblc.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3fbncxlaa.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3zjlawwrl.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3pbsmsjky.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3doiybekb.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3wlrvetae.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3lvybletw.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3bppfaqat.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3ucrkxyfm.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3xmjkkfwg.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3mbkimvtw.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3rrannaap.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3bvlsdwcx.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3lhqgypkb.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3wavnpiqk.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3mbjvbkks.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3xgngzoty.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3zbplsdca.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3mqdghwsn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3pkxjzuhb.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ywecascv.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3zcdfrosi.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3fykvbcgg.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3hosnhcvo.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3nuvncilr.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3rcnnofnp.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3ggxabxqv.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3njzpxqjd.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3qjlkzylh.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3mkveeuxw.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3avzncuhk.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3ljcolqjc.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3gdnskptm.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3eplxucam.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3qgzmejer.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3xhbkiyvk.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3xtjbypqr.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3mbetkekq.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3duedxtyp.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3qeizbpmq.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3kifzwbhf.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3jtkoevpy.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3xevkbsrw.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3bdevfosk.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3dcybhzso.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3fmdfdapd.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3csrakbqs.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3lfkohqen.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3gnewpxtf.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3rmorlxgm.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3zvetlsfh.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3tpzvidyw.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3rhuquuko.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3snkzxerl.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3fkigbobc.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3qfzsazub.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3pfgusszg.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3qocoiziu.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3lghpbtsa.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3hlvikrcf.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3glxxxvtz.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3qljkefxr.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3zmmzgdgx.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3cqisthoc.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3rygsnymz.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3tosyhcic.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3mycmfedl.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3eseswlvg.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3tezvqyce.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3yuwhtohw.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3xczppqyh.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3jmohfnvf.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3bervntlt.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3bmmgrrhp.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3buspwhxn.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3ndhidosy.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3jmchgckl.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3sgvwgwys.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3zrrtxkgs.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3zmkyqmen.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3axzdvnxi.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3omxfglcy.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3bdqzazps.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3hyvfmpzs.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ajxfglac.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3hjcmyfqs.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3ipenzdpf.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3mmidciic.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3jwdzwbdu.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3wdkfpikz.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3cdljrzhr.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3dbjtxvfp.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3jtkxkgel.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3ldhbhbgc.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3esyaxevn.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3mubdgyeb.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3mansavfi.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3ayedffse.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3lsuhnwnu.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3mkdwibwk.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3uxzqsmpx.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3zqcxfaux.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3rjjsocqr.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3sgtpljkf.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3icrbhiis.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3huwxmfuk.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3chknrarm.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3aflkosbo.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3zdmwsdgg.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wnmizemi.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3dwwthytz.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3ezijzdsj.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3xyatmfdq.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3qypohrap.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3zdxckzax.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3vheanzvk.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3fhxfbcfn.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3evhhebmq.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3kdnpmtis.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3shhxcicw.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3hasfpuiu.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3gkhjrtcv.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3gbmecrre.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3lhumnbkf.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3gdurqgme.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3upuorbyt.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3jaktfnwi.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3apmjqmvg.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3rpavjacf.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3naucdqcj.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3aedvvxpr.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3jerstplo.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3qehmzwhj.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3ezqfxkls.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uhxoxkpl.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3qxszwobj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tgkcvslr.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xfpwxvfb.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3ullfjkkz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3fzppvhwn.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3wbgahfqf.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3emdtpcib.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3ukjltlsa.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3wqfvlyul.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3bnhhmkje.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3uqaeculk.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3tlowhfeb.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3chybuibp.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ofrfspfc.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3fxxtasid.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3kqgyifpd.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3yxdqyqmz.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3jvnrsxeq.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3fkdfxmrg.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3pawvbtsa.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3cbnerjuj.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3abtcrkro.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3ltyxvvev.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3dhrijgda.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3galrrvvi.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3amlpilzk.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3lzmdscpv.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3ifhzelti.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3kpgzhflg.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3sewtqbaw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3tgyumznm.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3lmffxlzy.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3vryfljqq.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3myrqrfeg.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3luqectts.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3knqmjjls.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3tnuwmdcm.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ntuedhsf.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3cefcddan.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3mmrcbzqh.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3pfwbklld.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3vkrhxlvb.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3yhzgrfca.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3khbrfgtc.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3pspdsqgk.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3kjyilyux.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3gpqeiuca.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3gchvtebv.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3uamwnlfd.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3naysjyli.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3wpmwhuju.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3ahgzwcmj.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3patkcjkg.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3dlmgeqca.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3nhcmfbfs.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3biustblk.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3jbdkcuur.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3lduyevsl.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3gkbuakef.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3hjqpejym.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3kcvtywrj.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3zhoukllw.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3uryzywnf.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3kwpuvsnk.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3kaxalfsy.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3sxqlevzd.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3sqcweijj.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tyjqnngm.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3osqplriz.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3osocozdb.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ohpfzvzp.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3cfogcubq.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3soxenmbw.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3hvlbwkuf.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3aycffltd.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3pnlcfeeu.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3vhbkjtls.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3nazmwflw.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3yowbiavv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3zgbeaydx.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3hztgxamv.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vowiraya.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3wibkxjnj.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3uhmgfhxm.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3gdhqvylv.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3ptqsyvkf.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3iyqwuhdw.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hzsqbgku.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3zbiegmvm.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3qxgjgzvz.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3afusehya.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3fzcbsncl.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3prhupduj.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3rbxytmub.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3rjvyjnpe.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3zfncjpqf.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3aqdcgiyi.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3fdgvdirk.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3kpzdslqk.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3chwospkh.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3alantiwc.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3rqscokps.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ppacvrwe.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3wzfpjors.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3bsbgirpk.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3ydahwifa.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3ydjiiflv.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3wlgyialx.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ncymkrfc.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3tacnjvdr.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3jqgktygw.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3qackmcsn.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3kvjurvkl.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3jiwuijys.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3ftffmpqi.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3whwrtysh.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3ngpfbrim.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3kbgqebuf.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3oveqpwhn.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3ipcunodc.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3xnppkvnn.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3yqtmrwqr.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3tfbmebqn.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3hlgldgou.html


<!-- 参考信息 -->