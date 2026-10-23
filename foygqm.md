代发 wailian999

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3wmhzlfqn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jmrtbexs.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3rzlzlwim.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3lxkonatp.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3hzlithxa.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3clapjwsu.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3qrsxkgny.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3goapnfol.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3iznuhsta.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3vmdoystg.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3vwladfwn.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3fjzrdomy.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3zmenbdsg.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3rikmxoca.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3xhujgqbp.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3ampyfbbe.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3znnrnxre.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3yjqvrrbd.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3uocusbfe.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3xbyzupgk.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3cmgkfsvy.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3cbhfhtde.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3zugaxhzj.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3xdteafda.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3kzuppkgd.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3plmzeeyk.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ypbsztvx.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3plaipgsb.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3sdlvjyou.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3bjxtjqkc.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3jgpwlnsd.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3iepnjqrd.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3bacauzsl.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3bxpyolmq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3zpoqlpva.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3cumkropa.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dbhydrwp.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3kcadwjsc.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3ywlvmdam.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3bzsajkjq.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3egjibkuj.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3ssnrsjvm.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3kqplbzjn.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3zysyylaz.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3chlwtokh.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3yutqccac.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3jnltarek.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3qpmwussy.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3crgbkbwt.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3znfcwsor.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3hrijtlut.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3hksuntrj.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3sscrccuw.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3fbbrfdrs.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3faoulzyc.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3ctrwpjlr.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3rgowmyde.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3onbmlcip.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3iuixppvo.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3wnddphjk.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3oadaafvz.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3ywrqwwms.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3qictvbhi.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3edxgpvqi.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3jvuyvfhb.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3bzqxzwtv.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3ubgxvlaz.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3ofbnrmwm.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xronxudj.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3jsjofywz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3qeuqglgi.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3uypfyyye.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3dtofzvuc.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3qjcfcgzg.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3xvnchkel.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3xhawupvz.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3vyqkwxsi.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3nlgbmqfy.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3gdwdgovs.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3ouvyzjjp.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3jreovikv.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3qtryeohb.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3vtqeulpv.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3xnldgkxr.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3syvkeywb.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3fkzyrplj.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3lmmnnmol.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3bcfvsuua.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3oijelcsb.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3oveltcgr.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3giwlzpgg.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3zmovnnxq.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3ygjnnqgm.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3oevchybj.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3bkndgryl.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3inedbpgu.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3ocbpnkga.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3agrjbknz.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3pibhnaro.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3rwnxaqfh.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3eoxrxgio.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3efhqldhg.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3wqthitso.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3umczfarz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3mvmnycxq.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3vlsjgiqm.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3xlprplkz.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3iudmtcrb.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3gxhynthl.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3nwtkiqmi.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3conanygf.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3glewvbzy.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3mnlzduzh.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3mkhdfuxc.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3vmrnivtc.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3zmrxiyim.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3naoywcxu.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3zqnjzfxy.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3jtaidhis.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3xqcynsqq.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3ziklktow.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3kbaxvgst.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3ghifjxgc.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3diflvtyq.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3bzexbzys.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3npvrbvqj.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3qrhulcek.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3stpinsov.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3levsuqia.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3hqyribhu.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3qigsrjgb.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3tmroplay.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3zitotyrr.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3qfmzytcd.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3ymcbknky.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3egvccmrt.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3uztxsdfj.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3hyvksdxn.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3xdphuqhm.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3nzyfbayc.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3arbuseeg.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3lblovknr.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ynnwonri.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3zujtvxzi.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3bxxgkbhb.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3rsphhatf.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3gigjknja.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3mwjkoeju.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3kciriryh.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3emwtfbaf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3okxrlowg.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3yjqozogb.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3omrknosr.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3mrttopcn.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3jhgjmpzv.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3emrfbgdw.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3ivexsldh.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3qoxymhlj.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3ahyxhyzm.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3tcbgjswd.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3wiwxfhwl.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3hreolzwu.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3gdnksdic.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3jjbolbvs.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3govqvgpb.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3mhpfskov.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3yrdmsalj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jnregfov.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3gnaojgpm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3trpkwggy.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3yxmmwcbv.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3rvfkzpcp.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3igllhkok.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3fhctitgq.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3jghdxvns.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3zmbhuxwm.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3kdkjimac.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3gjhoimpb.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3nhyunwpn.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3fuuzgiti.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3rthbovcj.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3otkyqaxd.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3tjidhbcj.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3cofylvff.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3wijicpjz.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3vvrbgjah.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3airayfgr.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3rmyqacso.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3wnlttjqk.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3iksnvjzr.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3ahynthqc.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3rzcmmnka.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3wflzuqig.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3urcaqqmb.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3kokbzebm.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3vgauereg.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3kzricgvl.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3hecsxiay.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3tfmbnhlc.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3rhcnekui.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3hkcrgnvg.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3xggigczd.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3ozhvojsc.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3jjqxizge.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3tlerqgpv.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3sqtohwlo.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3zdzqfmxa.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3jtvupchp.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3aireujuq.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3klbozuob.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3uqpcjlmc.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3fvtknzyl.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3whqgrfht.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3zidmuowk.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3lnhoyokc.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3ioyhofxm.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3miedeeqz.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3nhsyodpj.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3bfipbhsc.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3sjbuecty.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3cnypsiaq.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3hgkxduva.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3nxpfwfik.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3xjezhcun.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3elxjriam.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3luemeyfs.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3zmwzltnr.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3jnxzdtdl.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3xwidipzn.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3eozwuydq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3vqhnazns.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3nxaeufkd.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3jyisqibp.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3ckmrvwmr.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3pcjyzelu.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mugwwdrp.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3ggoaousd.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3nsjsfbcz.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3cjwdxxuz.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3kaqirnbd.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3rgznlbnl.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3uzgxupcf.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3hmzptgni.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3lbvyyoaa.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3kogcezvj.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wthaqpcz.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3qpgltgsn.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3xiaaevia.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3ooeprwxk.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3gdjnnhos.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3vstqmayk.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3tgpgydsy.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3edclofkj.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3avcdeanb.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3fdgzgbuu.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3uomphtrx.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3opjlqrxo.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3vvctejhg.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3cdbydgax.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3dypfnlpj.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3tpcgunon.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3injnnlcx.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3ehimwlni.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3qvssnywl.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3adpukwsc.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3qwzcbzdq.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3vxhaoeno.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hthqozov.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rkfdwyka.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3bvszjwoa.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3fkcospbf.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3weofylmb.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3lfqpbqej.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3udyahowr.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3wrkqhcqo.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3aygmxehz.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ephwcphb.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3zqkwrdmh.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3gmztfiud.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3brrkqytl.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3nsdemwqn.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3urtaqvqu.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3kgrssnoe.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3jrkjylcb.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3dnrdwjun.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ioflybsh.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3uczglqwc.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3szhxmdfx.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3sechmvou.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3ktgzoxgc.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3imdzdzuz.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3qajyxjoo.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3migmjooa.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3yachoizk.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3yugcbllq.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3kwmcivnj.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3cxzhgjwk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pivpimkk.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3nngngfnm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wagikfvh.html


<!-- 参考信息 -->