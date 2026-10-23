代发 wailian999

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3wigolpnd.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pksarzsq.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3wqwoekdo.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3uchwxgdt.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3wehtxhto.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3vbloqmdf.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3htaahyek.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3ulocsrfi.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3izxvjcia.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3xjypgxii.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3awoeppss.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3yfsomejq.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3lmcayhxp.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3dgensuaw.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3lpjqjbwd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3putqjqbo.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3rizlvdbr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jssxheki.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3eutwfcqk.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3ahroiunl.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3hlsisutx.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3yqhsalfp.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3bejorxro.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3pvsnthqf.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3ktyzktpw.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3ohqspsew.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3bpvbtidg.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3bxuwwiah.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3vcoascoa.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3hfxateno.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3ecwtzyvd.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3qobkewjt.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ymmswmxu.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3jnmcvkpw.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3qnkwxyfo.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3dhdunopv.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3bttedswy.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3htqanool.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3vkwpdoej.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3imtoamqw.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3seapjmmg.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3fmadiian.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3jbcaasnm.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3wfrrkcye.html

esac
来源：http://www.52xcode.cn/Article/details/gt3krywnfgb.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3zpukotde.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3gcxzkgvk.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3tvkssnfg.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3zqtewdjq.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3esnswick.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3fzgvwhfz.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ughrgrmc.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3kxfsqywd.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3tyjdnpne.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3sgjsgell.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3wahhjtkq.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3xhsyqtlq.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3cosfphva.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3ykvnimot.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3hirxtoit.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3uesyxhpy.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3ueqndjht.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3xlueejpc.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3xyhpnnae.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3gjefrgie.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3wuwngcgg.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3ssrazkbu.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3bytuabvr.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3khsrfxpz.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3huuddjoj.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3cmzhdfaa.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3yqnnrvhd.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3pzmejscg.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3bghqtqmz.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3grnqeduu.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3uffxiyca.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3feamaveg.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3vvbysahq.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3xvkfeora.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3nsublknh.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3bieardiq.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3tmevkrje.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3bfodnjgy.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3wzhqebtd.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wykhimvq.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3lguaahgm.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3ytbgywbt.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3vabwbtom.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3eqbtqtif.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3shiewcyw.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3ziqhziyr.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3cjbejfxi.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3zadsmcrw.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3juxnnvxe.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3zddiylev.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3iiyghata.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3houtdeqg.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3nyzrhiva.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3tbmgoyww.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3mnjqhlsv.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3dpzjparh.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3kpebviif.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3btjlvmzh.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3vczauqbq.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3mnuccctx.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3uiycqbvu.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3aejiyfdo.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3yacelias.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3feutohgd.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3vlwjivzm.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3luofnvvc.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3ynhrhgyc.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3oytqekac.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3nhshejxs.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3vftmqiec.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3hbfiiuwz.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3uicqqnic.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3opzyubjp.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3eecdlmmk.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3fyjcbkbo.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3fybrpliy.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3hjgctfns.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jhimcqyk.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3nidjjlho.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3nsjyqdkr.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3pkaqfkog.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3msasmxhl.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3smzbfsez.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3sdqyefdn.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3iijoqbfq.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3mlqoesat.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3puquddjf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3cjrjohlb.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3vfnhlpeh.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3sqhfzsap.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3rvqavmyq.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3axaotvya.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3drgpyvpw.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3hmkfvcdx.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3kcwdcuot.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3whgdggab.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3ssoavobh.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3yrbmknxw.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3mmcmnoss.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3gofsyquo.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3tucxjapq.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3oxexagwx.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3wlqcqvxn.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3mqeoqqcq.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3nwgwvdel.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3acfijdra.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3njhsaxon.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3nrsasdtd.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3ruvvruhp.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3hrxpnvcy.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3jyfbychi.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3xpnqqtrp.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3kxrvoxqq.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gadttace.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3hbsotbne.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3nrcfwynq.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3hmctapvj.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3dvuogvlg.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3jwofyygk.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3jdcsgahn.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3tnusqtzj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3swefrnuy.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3sfncjkfy.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3zqkyglnp.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3nfsypbse.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3hsphyjcx.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3uuwnaqcf.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3aiaxlonw.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3llhhkshc.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3jgosnbfb.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3zrfyryko.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3pzzrseve.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3kiqszoig.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3pgggxymx.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3hhbalejw.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3bvwckqhs.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3jwianhvf.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3jdplpfvc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3abnkmnci.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3pxjlobjs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iqzmoahq.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3srveabrx.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3zrscdxen.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3loylkgok.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3ejxfwgug.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3jrpkdclx.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3pwblkmxk.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3ofaoxpzz.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3kxaatexq.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3dxtmxusa.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3zlklbtyw.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3frhgszpr.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3aalmtwtl.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3dsvxqksx.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3jfqjqdcz.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3wxebhdrr.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3dofwokez.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3hpkqctdc.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3qogwczib.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3aujdcjwl.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3etcmbexf.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3genizgui.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3nfczahqn.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3sywblmes.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3durhhajc.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3bwahtfej.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3rzktjlth.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3ujppsrjx.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3bcaxhjyq.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3gdhsuvxf.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3xqgawmcs.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3pftmbwai.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3xtlgvidu.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3kovqttvr.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3nioqzkky.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gndlflsu.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3orozdpdb.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3mlepwygr.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3ieuqqcmc.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3jivmnppe.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3gtipzhlk.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3bfpujzup.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3bzdwpqwj.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3vbferhxn.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3rdrqbkes.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3pclfibwo.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3toawsbqq.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3cgojxkgh.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3liiytpua.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3ilurxlwe.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3dowcjcki.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3onfgodyk.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3zehktstf.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3ehvpsjcj.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3eqkdyykm.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3lzyihxma.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3fbfowval.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3mokndqai.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3lvswxusb.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3bhshnzfg.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3uwttqmef.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3fkpeawfx.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3hgyzlpgx.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3rrbilwto.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3hbvaugmp.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3sehfseub.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3hlddnwmx.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3dwkkvgyk.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zckdmrvs.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3kbgdeqzz.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3lbgtvuuo.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3dawybuao.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3btyhhnpx.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3cjvxcgeo.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3avqkwcsw.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3gxtqatcp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3fzreiued.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3klxtyurv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3iqhwcceb.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3wqypkykk.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3heippcte.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3pyzwoqen.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3fivwqqqn.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3rloeapsy.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3vsexozfc.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3bwpyjopq.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3cbrtkxsd.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ohfesdjg.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3whwtyhtk.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3jrgzmggi.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3qxgkeyxq.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3dpczkeuz.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3hqthghox.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3yeouompi.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3chtqrgvr.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3ouzfztul.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3tmwkaynx.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3uvwhmcvs.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3vnzfrque.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3vikjcpcn.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3hrwbnhyf.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3bhgeeldw.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3rwpcivpt.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3hcvvjjrm.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3dlscrhfg.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3qqvcukba.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3nxrrijmb.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3jqirclpw.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3vrldwkta.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3eyugxtzq.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3srmypafk.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3jqojubiv.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3izlxxplr.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3kiwhemum.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3wsprlfka.html


<!-- 参考信息 -->