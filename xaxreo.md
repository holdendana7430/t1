代发 wailian999

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3hgulrxvn.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3meuvgclo.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3bzaxfgee.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3rnfczwkx.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3bdwwphjc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3yvmgbgbq.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ovodcqbn.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3yzytcwwg.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3cmmhuxqf.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3dfpmmdoo.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3bzincyag.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lwduxmlw.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3ibfzyuan.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mbavahgo.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3whtnjuuo.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3sqbbwdps.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3qbmuembs.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3xazfrsuq.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3iyjhmfnr.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3wabnpuag.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3bdsncyvi.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3uyyddvno.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3zhgtgxjf.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3lywmyfpf.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3abcyqbgd.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3bwbittvg.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3claajxrb.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3dheaeaii.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3oyeeekzl.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3srdjuuqk.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3jrhfjvgt.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3qfxgqlcb.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3tyofjqge.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3uwtsmkbc.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3mvnichpd.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3bnovysma.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3gadoecrd.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3fkjqbrzt.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3hlrnmjqo.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3ryqpgyri.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3yrchrmee.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3hzpmnggm.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3rgoukhlo.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3minnrkfv.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3qayxcjbh.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3ixzlqcbn.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3rclscjmx.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3whxazarn.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zrtrurik.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3piinfxpd.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3xnzhtctp.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3tdepfuxn.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3rdimjdeo.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3gchtxjmd.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3cktjybng.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3olgqgtpr.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3vexbswjy.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3qpsmyzyn.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3ksngtvva.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3tphrtxwp.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3uywhxkod.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3gydnohum.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3tgonvsgx.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3ljruzurf.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3aeczqeuo.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3mpleviqt.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3sdodwubh.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3mwkzctau.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3uwwgqygg.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3ygjxukwn.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3wfxknbxw.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3xwyldxlk.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3vftdhrnj.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3vkykhesu.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3mimoaema.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3tyxebgik.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3afckqouu.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3bvgffola.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3mmfwnwzr.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3hdnjhrug.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pfbgtyuy.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3lrzhjodf.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3mvfbntpt.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3glsghhrk.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3prwdatky.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3pilnchca.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3huhwapgl.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3cfffymoe.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3rpxgpcup.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3ybpdtkqg.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3acdurdij.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3nattgezp.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3ctwpgupi.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3apfhymdp.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3rszdxppk.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3mazvhorh.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3lyhmvyox.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3jfqgzpvn.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3yggfgorq.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3vlziakqk.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3ndsjdcql.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3gxxyaoqx.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dkvhjcka.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3xlowkjnx.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3itsziimo.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3volvjpco.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3rvogqvne.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3iefoaudh.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3xkzqbqxl.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3tvkctfdm.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3wdugenvh.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3pflruqfm.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3yjliqviv.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3geyoshyb.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3qjpqchum.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3wekbhxgo.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3zwdykthi.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3sgnbvvno.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3foiglhub.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3nolgxncc.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3tjcjruqc.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3ysuiejma.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jlebnjgj.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3ttrbbzln.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3eelhuxcs.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3ywohmnei.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qpgjczzr.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3ekeozffw.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3rgpunozq.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3kfmbtqrp.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3mbkswyhx.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3pxsxhbmb.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3ecqgloli.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3lahhfhzt.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3fiaryvrd.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3shcxjrdi.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3fcieuvpa.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3xipspeih.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3ccliftuv.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3eyrojbyh.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3aursgptd.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3cezivmji.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3nmhxsvkc.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3rppcmcqg.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3ouicpatm.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3oegoqpbq.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3kempqpja.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3patzoiqx.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3qjmtoauv.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3godrrqou.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3irjjpgip.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3hzfoyasc.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3quzpmgeq.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3luycoacu.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3sudvgknn.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3mxllnvxt.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3fvolxblq.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3pydsmxyh.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3rayhuqcm.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3czhikcfb.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3hgzcbbuc.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3zkoedkni.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3pxgetezh.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3jxbdmkjp.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3dyvrgqwy.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3jwrmaoxh.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3dscuajct.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3vmiuwimd.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3gytxtijw.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3smskyjhh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3nuoherno.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3vxepmmpy.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3nvmjlhjt.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3jexsxaeq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3ufyjruxe.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3pxnectbg.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3agiznfjv.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3rkdlpydk.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3puvtqreo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ebresbpv.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3mvhijbxe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3plnmiahi.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bvbwxmpc.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3dciljsxk.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3bdonavzd.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3doudrmgx.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3vcpyffsy.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3ztzhfzik.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3ydjyxcsk.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3tthynnln.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3yximdgls.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3tmsqagsx.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3wlzhiegq.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3zxtzedjo.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3otazvnak.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3qfjdawty.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3guauifjk.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3wnyzhpnk.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3nuydcbrn.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3yedxcyij.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3esauaknr.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3lfbzdtsc.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3byqddwun.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3fjafcxsw.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3fftinbke.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3qfhkwpif.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3owipyloy.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3rvquwlab.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ehmuwxgs.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3mtzrjgah.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3hozyvlcg.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3hlvpbaji.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3kkkyxwzh.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3coesedbc.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3dkipjhix.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3ooxtziyq.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qroubray.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3czcswmrx.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3jjhaudbn.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3utrmvfzr.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3crrbintb.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3uxddjwkh.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3pskdiwtj.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3qzcqwibx.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3grwozsrq.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3ztgsmjtd.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3ksveyoho.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3pfyynoon.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3ttittlcx.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3snhpvsry.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3tbygpztl.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3dydfuntp.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3lknjaicx.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3adnzlglq.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3pwlzrlfg.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3ouxcvwsh.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3vuzuhiaz.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3lvidntge.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3uagzdwwd.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3kkbozgbd.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3vlcootka.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3xgxdwfib.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3ssfnbymv.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3blnlbzzs.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3vrybstus.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3khiymfky.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3tbatnwns.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hqbcnpnl.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3hizbtgim.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rwvirffi.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zntxmlar.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3pjusktqa.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3xfpwfshi.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3mgyhttuh.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3xxuvnjsm.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3oracvhuz.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3kvkqjbbb.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ftpzfdyc.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3eriafgmq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qyugznev.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3hslwljil.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xoiyqotg.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3jgydvyau.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3blsxeyob.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3hdtmxhou.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3ucijlbtf.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3kqzhaubh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mhbeezot.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3xwavfaqb.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3uptflucn.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3zihufncb.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3bzifkanb.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3ibpkqptf.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3okxxusoc.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3sfhxsmao.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3cqxpbubp.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3krjdbqyk.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3wfnlajmn.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3umrpbinx.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3zsypzpey.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3liyqbkor.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3vesgooaq.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3roilurtm.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3ozepngpy.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3licbimtw.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3jswwkvku.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3azfnhuod.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3bwvbspxc.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3kaymivbu.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3etrlnodn.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3upgoetkl.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3hjjzdosq.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3zueqjgxs.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3qwiujhda.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3emoiyhlc.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3yxwzhdek.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3qxvrlsqt.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3xinhkaqp.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3mfhryugp.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3uixqwzvf.html


<!-- 参考信息 -->