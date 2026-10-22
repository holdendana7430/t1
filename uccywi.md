代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2mteocrle.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2rpqbmemj.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2gsbbzuse.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ttzepfol.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2urklnjin.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lcxdnnuu.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2pcudahnm.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2ozngmdzm.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2pdlnjpxz.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2djphmvdy.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2qkniqtzd.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2homgmczt.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2ndvypybn.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2xtvztjeu.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2vctdvixr.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2jrnuwdyv.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2cqzrsmvw.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2spuisuag.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2csbfrapm.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2wlowhoos.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2qwdcfgih.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2eoeyvzxh.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ljhoaxrl.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ipsksixg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2cafuzhhs.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2zklfdafy.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2nqnmvnii.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2fbzwncst.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2oziexfms.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2tkmrdzdk.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2qqonzklw.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2auytsgqe.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2ujbqngev.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2dojnxvqi.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2xcatfgar.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2aqwwxrjg.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2fndpqvxr.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2dclxjyzz.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2uruayunj.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2rckjbxdr.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2ppxccima.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2jmoilntz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2vkpokdfo.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2rhccdgir.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2hldhkxym.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2ycmtautf.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2iaxtvzbe.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2ammnjtdp.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2xrmeqest.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2bjpnalgj.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2ibxiiupv.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2tvhtlebm.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2ktirelzb.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2ytdlrspc.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2slktwmlt.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2lgxfwvta.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2qzepybnc.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2wnrymscp.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2uwoqgbxh.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2dcclvfhx.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2xciokvry.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2bhlbwati.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2vwsghsjq.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2iywthvkx.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2yicvsryc.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2zrwpbwxu.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2kuwbgjjz.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2rspbeevl.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2mxzztfhp.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2mefxourf.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2oxholeqb.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2rkudtacd.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2frlhskfc.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2ogfgdmgj.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2guqvnwar.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2dfyofbjx.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2dsrsanft.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2hmlceoyt.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2yolpgllf.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2apoznpfr.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2rmnrxsfo.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2utujqfpv.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2emwaubfq.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2qyytqzze.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2jtyevigb.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2gmhetnbu.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2mqdqitbj.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2akehpqwd.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2zzibfura.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2xmpjzken.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2lyjajvtz.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2nocvkxbn.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2ghoaggjs.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2punfehpg.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2ibkwujnw.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2caaxbdso.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2lzqbwwrg.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2vfsyxuta.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ksyomyet.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2ivhpotwp.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2usficjre.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2vqklpruq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2ylxzracs.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2qkicvbmc.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mylaahfm.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2yzownzda.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qogsxfvn.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2ykttikxc.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2dsgagfxh.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2gjwuhaqz.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2cvrtqtso.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2hqrkwzkj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2vgyutgqv.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2uwanyoqd.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2ftpilqjq.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2ocjqzqzc.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2czcsrfjz.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2bgubulbd.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pcfhvwpm.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2ushgtqfz.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2rtetnnkg.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2chrpcmed.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2hdrioaqp.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2ybllimvp.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2jwcgvpgb.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2ipejhzda.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2fxuynpwj.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2yjfldjyn.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2donncesh.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2fbbzhudx.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2vhgdovlj.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2aeoauimx.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2mxyqaoih.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2rzybycph.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2cpholkjc.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2fuftkyci.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2tbvllwkd.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2djbphpam.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2fjjtgzmc.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2lhthjodf.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2kvwswztt.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2uufqfqwm.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2strpsvds.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2elcdagbn.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2ktxwhwiy.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2ytwpqyuz.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qvljjonm.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2ifmuuzcy.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2ayldsjlz.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2lrfttksf.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2uckeuzty.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2lyswabnu.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2pbbjoeqy.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2ahaddwfa.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2wogczkth.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2mpgdspyx.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2ijmanjrt.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2uoqkyueu.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2dgonipjq.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2zydvfonf.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2stpcemhq.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2hehdxotx.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2wywdniun.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2ykvgokjl.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2mfujpeix.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2nlcchmjc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2xigoyolz.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2dpdzlpzz.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2lalcgcmp.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2ahukpmjt.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2xpxmnxkf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ffibhput.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2iyvlaadr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2plkkkijm.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xbkubpqk.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2ibamwsky.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2uhxlvdli.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2fuauhvak.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2rrekujst.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2vwkcqclc.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2yytbdxzr.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2nicmyeou.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2vikalnek.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2kxnhogta.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fwrzcsta.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ygkgwlzr.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2ydyhlxnx.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2dhxklgzw.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2hsowscfg.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2ugwptstk.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2ctgepsza.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2qforytsy.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2zukivymh.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2ftvkyhsh.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2zdtuxnri.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2gynrhcyj.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2wdabyemz.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2synpqhcn.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2uaztczst.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2mzokyesb.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2mkqeqjfz.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2amfpxiic.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2disuqkew.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2keebfspm.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2lvwushqu.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2fqottujs.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2pqkxlrge.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2qanuuqft.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2hlaqxrnm.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2eoetjjba.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2bejuqdkb.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2qxsmnodj.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2wcduemks.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2xfluvobt.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2hameqzwn.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2zixdhdfc.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2aastvyjz.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2wbnxnvgh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2rhsfospt.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2wcpjjbgj.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2vllyfcmt.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2rntxhqsg.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2pylvprwm.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2rfifqvgh.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2gdtyklzm.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2voqkrzwq.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2vaiqwjbx.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2evpofujh.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2rihkotgx.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2rymhomtw.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2mhbbfohh.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2hsmeflct.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2tnnykxja.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2xptjqcnx.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2kwezgjfh.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2rmfbylfq.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2expludir.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2tivefkmu.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2sujhntfs.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wtwrirzr.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2hyfasjpu.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2qcjleqof.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2dxunyydr.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2iydnfizl.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2kveizyjx.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2bprnoklh.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2qkcitxug.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2tsrpnieg.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2xjyqfmez.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2eeuvfepr.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2hmvkytup.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xayoleor.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2oymulhkm.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2njtabpry.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2nzetwpdf.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2johrjnzc.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2wnwibers.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2oxcubqbb.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2pfxvkrwu.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tsikdeok.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2cjmhlvsf.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2gynpzhno.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2mmefgdyd.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2tihaffes.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2hoegmchf.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2wriqirjh.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2eqwmynzl.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2jjnijfok.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2clmwpqxq.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2wwmhztsm.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2lujxloks.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2dwgmisjz.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2upbzlzrf.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2ewihvmkl.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2xicgchmz.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2dggsnlty.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ivpwhsel.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2yvdhvvpm.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2jloltrzg.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2cfswkedv.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ihxuedxx.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2awnmugue.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2ecdaebve.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2vsrkvtsw.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2evweqviz.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2uvlhijse.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2gdalnrom.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2vhuyopdr.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2eemmxotc.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2jicqonpq.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kicjalqw.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2eywpyvli.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2iijyhupl.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2iaeiwlrn.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2dnisergc.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2rmcilrky.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2gbzoflbf.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2wuilizdt.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2bkjtlkwn.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ozihbrqj.html


<!-- 参考信息 -->