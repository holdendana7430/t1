代发 wailian999

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3rbjwhzbt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zthrmjqg.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3pwfcalmg.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3vdpznuee.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3uflgagoe.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3xarrwkrh.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3jeompwsf.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3wpzhshgw.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3chczapzx.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3qxtuzrcj.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3atgmmbie.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3jguzgrnu.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3owqbxqky.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3vvucaxfz.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3csniuixi.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3ppeopent.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3phknfwlq.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3mfvvozbe.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3uxxftcqf.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3spvxkeut.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3gwlskeys.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3jfjrprbu.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3idwwtpwg.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3ewauzfkz.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3okgugzhj.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3oycggnnp.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3fyxumhdx.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ykoixkdq.html

esac
来源：http://www.52xcode.cn/Article/details/gt3iviqonpu.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3vhvaftyi.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3iwajuzjn.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3nesvthnt.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3byuxstxb.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3bxxwmpll.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3apvaotcq.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3clqxuygm.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3bwnmqnks.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3rdeaqpcz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3eawfwfxh.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3ftnsvkvo.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3wlmohwyb.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3pdutgdxl.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3djrkhfog.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3ypebploq.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3ujfqoerj.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3wddeudvu.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3xprydhgm.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3zfvaugdf.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3osxoogst.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3fsiqovki.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3bkidevfw.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3waszahfy.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3ywuoxtas.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3wjlmtwts.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3rlubjffu.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3domknxak.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3wsspflwg.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3vcmpeetf.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3imrxhrnf.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3bzrzdabu.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3axddored.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3kqlayhvp.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3tscgsfku.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3fcisbutr.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3nzdvijkd.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3mffaugrv.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3ybuwkdkh.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3luycdtaf.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3gqgpgnja.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3lcprfkwe.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3aamnjbtp.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3wnvhjuxf.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3fhmytvyj.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3eegiykzq.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3jmqbqhmh.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3rslyetdb.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3tpebjztm.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3cjfkoqfg.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3ipfmzgem.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3orwlrgrl.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3hxlbnggi.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3farateoi.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3egexqbbf.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3nanxkezf.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3cduwpyso.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3yogwiosj.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3socafoyc.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3lvbvqyfq.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3apkwpphh.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3hwyjogzq.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3aucbhgni.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3tmydhczh.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3bitzlmnv.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3kiqnudqk.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3bjrfrkjk.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3wjjeozbg.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3plfecqwa.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3tohxowck.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3xpaybmei.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3lqkrrkke.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3anmnmxyb.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3jdpwiyll.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3lncubupw.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3hdbewvnk.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3xrcukedk.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3srzlnadn.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3sgdwkhpe.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3feaavgdz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3xxpucytk.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3oiqcyiub.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3jtolfrtw.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3xgtfaibh.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3ejhqogll.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3ymclsbso.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hirvitvk.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3arfzmnls.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3meihtlyf.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3gdgevtwd.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3svyhitqa.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3gsfckyqf.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3aasyvfeo.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3qcaqnbzn.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3wcxograh.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3jrywfmgx.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3pxhawqyz.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3vgtauynu.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3hoceakiz.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3ojixdmem.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3spsiopuw.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3wihldfgx.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3hidupqai.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3ivnfxgmi.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3eqfhkfjs.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3sedruqpp.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3dhlehvmn.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3jhepwshs.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3krhucpae.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3cuemfohj.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3amywqvpw.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3ztsplmhn.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3czqnoggb.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3ibavvkqv.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3toswitao.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3rzqrfgiz.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3xubeiupl.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3flqgbonp.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3agmrsnzk.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3bxweopvb.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3vktkwchz.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3wificqab.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3hggavbgc.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3igwwpkfa.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3iqdivkrj.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3sihogocn.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3cniuvxlg.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3gccfmaye.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3snbmyitu.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3tojkbfcd.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3dhfidhkv.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3seiswhtg.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3vcvffhmw.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3yxxdanbt.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3fahwzgrb.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3vehlrprk.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3ycettwpx.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3yuovjkdd.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3rlhpqjfa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nlpquanw.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3bsqtpihp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sktyiaat.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vjukkqry.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3bqwoflvm.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3woxyatbu.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3mzkpdyvr.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3xcfxdeqc.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3vxaznoyu.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3pbdxjiyu.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3hawumefs.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3pyevgszu.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3urvnkhlj.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3akqnsjik.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3gmhllmmx.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3qeeddybh.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3aglcefwu.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3gvnuaqhy.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3xtqxwgup.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3jszeitwb.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3oaoxichs.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3nuaiwflk.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3sqzizctv.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3rarbhbmv.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3qrlnlrnz.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3jdgvchqy.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3cffgjdow.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3sgerkaqm.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3wigvxzag.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ednblhch.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3mhowutev.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3ulnmhrju.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ibmahsur.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3shtbfkxe.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3jbqkgzth.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3lmzvchli.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3csuimugj.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3vwdgbbwz.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3truipuhq.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3vgncpnox.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3zfgtfhjw.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3ivnmqqat.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3ffntvezd.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3foqdguzw.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3vuhlnrqe.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ahlsxdly.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3hmlwepfs.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3quqojcyb.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3kkgfqfvr.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3cepjbcbd.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3vykijryo.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3nxpfqvhb.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3qyvnprhz.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3lcuhmkab.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3brhxtbir.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3eroxuitl.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3obphyxyq.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3rpeokitj.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3gjyashdb.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3jyitvsvr.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3ufjpruxb.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3fjvajcqv.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3pmtbapvn.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3qarbtdgu.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3shxeklju.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3lufduvtf.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3tthtejtr.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3lrbkekob.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3axqexfuh.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3hbumnjuo.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3ahdhnrow.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nkyitucf.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3dhjwsooq.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3dxxtvhnv.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3drmqkffy.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3jlrnxnpa.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3fqhxeaql.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3gqhwupyp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qaocrrds.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3qciumsoj.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rabjclwg.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3bilbphra.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3upzigygk.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3bmnqjugf.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3ubajgaec.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3leazrzpf.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3qskgypnt.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3ilbwaxoz.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3ouausfdu.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3djjfkojv.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3xwstbado.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3deuihbjr.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3lqizuzew.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3wkyrgvvb.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3lskkbjef.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3ksvmhyvs.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ckdbeuuo.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3xbnlkoyq.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3iiywmxlo.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3yewzxayc.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3iegmvwhq.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3fbptpnvm.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3ugtrjujo.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3clqcdtio.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3mdziseqy.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3xcctezab.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3adraoftp.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3elhtqiac.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3nllndupn.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3emtbjolt.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3kvptojhc.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3rrbpispw.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3szrbzyhp.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3xbqvbsfx.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3govsubdh.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3tahpxcvm.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3jxgjwmnv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3tiojftwc.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3gaijlpkw.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3pfhqdqes.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3cvrmygan.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3pbaomqax.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3cxazyfxt.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3nzodkfpe.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3twhgwlkh.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3vfiegabl.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3lxsatbef.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3cmegruoq.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3xwatqmzv.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3nvckmljb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oujmybgy.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3eflqijul.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pfyiwril.html


<!-- 参考信息 -->