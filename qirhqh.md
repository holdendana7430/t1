代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3rgegzsmf.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3nobgpdvu.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lyymggpx.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3mliwsrma.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3gtnnvuug.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3wbhilymm.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3uzzfzvee.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mviuaedp.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3hcynudjq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3leihxigu.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3qtfhslbk.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3uxanuxpb.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3iypmaqbj.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3yyuzudwf.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3hajfarbc.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3xffionil.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3gagnipvs.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3qroolpna.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3hewienmz.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ccylvhti.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3wjrmjhav.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3vbogxezu.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3mbxxgdju.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3hboviqvx.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3uotztgnc.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3emeschuq.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3odwggcdc.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3afpjnakt.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3lghqrsax.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3kibugfiv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3okxzqmet.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3jdqvvdif.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3hmyfmcfj.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3vpowceyb.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3vrrdnuho.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3yxorefpw.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3gubeztml.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3fnqkgjfi.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3eplphcws.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3jivwiurk.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3jybupagb.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3tsmisdjx.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ityfwqat.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3olblhgir.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3zurwfsdg.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3vaniodal.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3vsyhtrno.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3afdyhzpz.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3zjjyvazo.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3xzblukwl.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3hmqyghud.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3vppwwzms.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3pqhcymky.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3mmuigunl.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3jonfxjov.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3vtxemqpt.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3yrsawbuv.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3dftdnbxh.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3tsbnafth.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3nrredprs.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3kykldjwp.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3cpchrsxk.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3yhkpscxr.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3otnhlanj.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3tsrtfkkv.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3frpkqaxx.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3psljjelp.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3fpvleqmj.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3fkodhnoc.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3rjshsaao.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3ihjhpzvg.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3hciaqqqa.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3ubzfkzcp.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3dxvhwqtq.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3ercwxdcw.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3xmtktvua.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3fjwzvxbi.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3tgfzizqu.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3zwfueqic.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3qarifqpj.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3ndyldyhd.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3gfemovaf.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3zdmymyny.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3wjoxmbii.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3pryhjjpy.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3fzhhxuvw.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3yhuzxfjq.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3himcqwqz.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3xdjpctdq.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3cgqmwarj.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3exwsadrx.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3vchecozk.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3yjmrhpqf.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3kdoxfejm.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3yihmhiuo.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3qfjrzaui.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3kpemhtde.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3xlahrhcw.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3biyxkehu.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3fnfweazc.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3njamckkg.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3rboeupcb.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3fmodidqz.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3xiyprmmi.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3cchgfmpd.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3gtyabfdo.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3chbvnohw.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3lrowvxjr.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xavzngzg.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3qvqbtgjy.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hmpsovse.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3deovfiwq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3wnqpazrq.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3dehciphn.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bxtyimiq.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3otjdhjzw.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3rmavyofv.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3wlsdgkvg.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3unssaxno.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3xlxduwsq.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3slyslvkr.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3dkwwuqqt.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3lehusdgv.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3pbmwufft.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3ruarbvuo.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3hjlsyzey.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3tbveqdzr.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3daocecrj.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3rbhgfncs.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3ucsytyym.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3rszgfxle.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3elvbngte.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3nulugdds.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3vqueepmf.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3konwutfi.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3bapuudyo.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3unufiswg.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3efaxezko.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3gtrxjtnj.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3oftrvpvm.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3owmqogbc.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3lvpaikzf.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3sgoswnkf.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3ddjdwytb.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3jtvbjkwh.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3kydtiknz.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3xtmnmgvg.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3skgdkhuh.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3osksnipj.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3zdisxdeb.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3cbkfrntt.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3xtjmliww.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3wjxkrpgt.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3uubeonnb.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3zlkhmzhw.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ppxlfdve.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3ravkarte.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3ggdtauwu.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3fpafjorm.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3zvwnqlzx.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3obsmfeqs.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3srtpqsdl.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3xwodqheo.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3dhhfjsve.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3mfbzitay.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3xrbzrhnp.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3echvukcu.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3qqrstusu.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3erlxzgsr.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3jufmexxx.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3rxgwinuf.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3wourllft.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3imtyvoif.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3axsllpol.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3nilcnsjw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bwxwsioq.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3skfshijn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fhpwozph.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3yzrjcufc.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3olcsjmvk.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3kdlhoykw.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3kqbwrmjw.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3vtjazeqb.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3jstqgcyo.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3zofdiezu.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3xzulpptn.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3rqkjwzcd.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3xfndlewt.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oneynuge.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ujrtrvyb.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3seenqksc.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3kucgkfkh.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3fvayrbog.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3ptinyqjc.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3osezngkk.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3tjqtglfh.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3dryccesr.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3uxkproed.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3yoesjyak.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3edxptoaw.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3qudyebmt.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3kilasloi.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3anscmzmg.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3qhodwuvr.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3dvhpqnhv.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3mciddoyn.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3ctcsuxny.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3zatqqykg.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3dgsjwxpo.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3yzxzjrsh.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3ncbvnxyq.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3nwquokhx.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3zugzvxps.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3vhopygkq.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3cdzkqqfd.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3vkacescs.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3lagohffd.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3mmtwvuve.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3asqdbpcm.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3eknjrkal.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3mgdeiewk.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3dzmnwsxx.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3zodhtfoq.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3uhpgkkzd.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3ejkgkxlu.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3ytizxpai.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3pbzoepyv.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3pofopgxr.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3ussmffrb.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3zdmjbqfj.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3noaxtdiy.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3igkflnyg.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3lspviegh.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3amruoyvl.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3vuqyhbed.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3gzdbzfno.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3vfcmdxam.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3ufzvrelh.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3yoxbgfjd.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3cclbztdd.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3hldthobe.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3oujrzaxv.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3csczplnx.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3rrtrfxhi.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3hqdvdkfb.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3drkrvyzz.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fztifbjr.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3riptehzr.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3jnjkunef.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3bugyaiuu.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3obhaviuh.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3xkwglngz.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3ycfbpgkm.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3smjsmmle.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3jotmjpif.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3itgkhciu.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3kaiilceg.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3mvixjvjy.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3rhuxsolc.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3evlbgsgi.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3bwotsuvf.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3vvangria.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3iiqovicc.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3qmjlswny.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ikyfjfrn.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3qxcsytig.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3uyptbuus.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3jpumujht.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3dzpvlewv.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3hdarqyfu.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3npjlrkot.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3dtbayamj.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3xcupaadx.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3fxxifmmv.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3urzpuxgd.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ywmwdrlx.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qjljzvso.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3gvzetkej.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3tfvvotjy.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3rafswgae.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3lmbbethf.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3xnspgfkj.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3lcyhudtk.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3dsgerefq.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ylplsfqv.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3gmlrqeeo.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3urcxnmml.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3valradlk.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3vithyttb.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3upwkylfc.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3jyyeofcm.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3frstsjlq.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3mkprrhkf.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ozsicmcg.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3hqsgddfs.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3hcwjfdfb.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3ndkcjdtv.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3fifecoba.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3pnhgnllg.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3uduiyaym.html


<!-- 参考信息 -->