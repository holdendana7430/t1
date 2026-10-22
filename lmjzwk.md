代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2kjcgbutq.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2licjskwa.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2virlbenw.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2sakwnftk.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2wqyxdxuy.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2ihdvbijq.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2oaanlaej.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ysszyqka.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2temgibni.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cwcmrijl.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2omybgdya.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2qgbuttco.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2itqdcziv.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2qkzmyfzm.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2vvtowbys.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2uobtpfdy.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2yfjemjee.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2qwyukoko.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2pcjeztnx.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2hevsjnbn.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2kfgwzwrc.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2sypuzlct.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2hwvvxdze.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2umuhujyi.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2gkfshbif.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2aiznwbqn.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2lmihoduv.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2msoqguzo.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2cbpacbod.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ddggwshr.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2bkktglnq.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2lqfsmnhe.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2gwbltvlt.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2markqxgr.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2fjasmixc.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2pfugemkw.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2pquchxgx.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2jugzymvf.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2seeingmg.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2fzagyems.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2zlladwhx.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2qqveqngh.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2hxiiuoit.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2jljpiplo.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pwftsxdr.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2lqehynpy.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2acacxrxs.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2lnrjkzzx.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2pzippzil.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2nviyvhhp.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2gqknczgy.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2lfdafelj.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2uzpmfsee.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2nrhmfnyp.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2wdjzvjxh.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2pmevteiu.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2cjnpnudj.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2gastxuog.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2aetwomdc.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2inlasrly.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2heatvqur.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2jcbpgnhy.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2lizswwrb.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2aototrcx.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2otqgphws.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2ibooedcv.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2sylofwne.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2kniovbnl.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2kouohbnx.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2kvtdrbqk.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2ligkjwum.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2mixthoum.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2drvbkzws.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2yhpvvosn.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2cgntlbii.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2oklgilsq.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2ujrwuwha.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2eykyqtyb.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2kidkztep.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2giupflqb.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2jelcqvrv.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2egsdbkdz.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2mylpkkaq.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2hwplyayb.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2roejkhpt.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2dvjrkgpa.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2jtloqctt.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2layeybaf.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2rrwecshl.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2glncwmdr.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2zsqxxdke.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2sfceifyc.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2uuppqbig.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2mcamplwm.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2fhisbfie.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2kbebtjdx.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2kkgubdaj.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2fslbwdsk.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2syrluhlv.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2thrblpjm.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2ndnnysca.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2worxxikx.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2vbazsisr.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2vmxndaen.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2gvxxhbvj.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2wbyiqfum.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2kngebsra.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2lnthnxpz.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2xdhgqbzi.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2zsnoyngh.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vasbwxrt.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2gzwwwove.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2lrwkevfk.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2zrcdopfh.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wcenjknp.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2tepldkgd.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2rrszxaog.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2vkdwolpe.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2thwrxzyl.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2rardeilt.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2oszfskuj.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2jsknoccx.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2qolifjqy.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2acmfulji.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2saawtsno.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2uwpplpjm.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2lckttond.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2drhguogh.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2pvnycrwk.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2iavkqgmd.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2syzkuqsj.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2dppqrpdy.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2jhlhekwq.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2wdcqqwnm.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2espzrnss.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2gbuyfyvk.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2vakvrusx.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2deqijyez.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2ubtyvrqg.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2sntufciv.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2npjxgukf.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2zcjnuadf.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2vuigrzbo.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2xeotftuo.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2lqabpksg.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2fzrfweee.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2wqkxnhnd.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2xscwvchb.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2nxqbpqwn.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2iktarckp.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2flcmkdat.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2xhchzzez.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2pnnyaccn.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2kiovvsol.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2wrojbzkl.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2lnijrrqk.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2aaboglpo.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2pscogrci.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2kynqbfxg.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2kmcyheps.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2xxceetph.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2iluyzonk.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2hyadwhgk.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2xbfsyxpb.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2rdymultn.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2eqwycdht.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2vfciojdv.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2klurwubw.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2pibfskyk.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2klysrkfv.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2cidsusmr.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2utnwzffg.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2sdirupwr.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2ynyctoti.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2ydwqzlmd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tieawpog.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2gzrhwttm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pttdznko.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2czwodcmp.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2yukbtvda.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2rytzqtal.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2exkbpmfj.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2ifaeauey.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2dgcpsygc.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2uebqyycd.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2iavvdclj.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2ayvhyjll.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2pmaoemdp.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wvfmnqyu.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2hphdxtbq.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2wxqqfzwb.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2nbfoflij.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2ddzgobse.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2cfmrhdad.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2yyxahvqd.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2coqdfrfz.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2xkysojui.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2ragkjuxx.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2tqzbcvue.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ffxaavgm.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2draqeytt.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2gmrogbdu.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2gduesmam.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2dydbplij.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2ojqiuggn.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2hrsykgcd.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2mmrsfgqh.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2dcdwmavs.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2ndnymbsy.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2nxtfzgqk.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2leqptohe.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2iihoimhq.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xxvawrdr.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ysdwbblx.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2qmohcxxg.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2swmjlojv.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2uefaeobs.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2ypdcabta.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2zlxqvept.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2mryszare.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2iluyvxrh.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2xycpvmow.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2qdbqqmwl.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2bepnbcjg.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2skdilfsi.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2oulipyod.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2cjefaecc.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2mxsjaeif.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2mbdcgkjn.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2lwdnogvl.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2xwbicllr.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2arnbtkxb.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2hsfjcjby.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2lrdvzljk.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2zdibndku.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2ylmlwllo.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2sebjeyas.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2elygbvqw.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2mlmbktio.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2lesiiakq.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2utfiiurt.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2fuhwsmus.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2ptmsbsiv.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jitfmuqs.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2klczhwaz.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2yjtblthq.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2jyaixnaj.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2nvtdoskb.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2hcvwtref.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2vpwwbefh.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2vbvmvtev.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2gsxfbnit.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2mmhyrxoe.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2voilqkfm.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2bpolriyv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2lsrfzymi.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2nnuiarfx.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2lbjwijbs.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2yycjrugd.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2uulckuoq.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2basujqao.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2xipdbatk.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2utmccrht.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2nkxvfank.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2hwaibrut.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2kmpnhpxj.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2lonmfndq.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2lpyvajhr.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2tqsiivad.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2wzxndvtg.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2iiqofjrv.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2uunnvxhz.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2yimwuoym.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2gwnnghla.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2byglfqvj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2iahapavc.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ybnpofxc.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2mhahtfms.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2axcbdnjs.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2ndpbxmjz.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2rtuckfju.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2svpaqadd.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2lgwbuezm.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2uowdfzsk.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2jfxserxu.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2fpgyucdr.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2nlgrlhcx.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2bunavxbe.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2gffjamnd.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2hfbmwaor.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2gfngcbyg.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2jazgwgam.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2mmxgqykj.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2nibpvwyd.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pclxbvgu.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2yxnwssps.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2seaicbyw.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2kdueymfe.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2zfmsivqs.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2etkcqnbo.html


<!-- 参考信息 -->