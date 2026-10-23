代发 wailian999

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3fwfqyyky.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3dmtrizye.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3fxfyunur.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3sgmuuzqj.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3ykxmehou.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3eoysxouq.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wwksvykc.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3ppwdiefp.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3syiylynu.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3plqfcyqi.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3akktjauq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3darcrqbf.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3vokroidx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jovkdirv.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3gzetshob.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3annejhbx.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3scauckex.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3eyhpydga.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3btrmyigc.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3iibarncm.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3jmnedtis.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3dbjulphl.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3fyefbxbl.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3bkzirdcb.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3gvqljimi.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3nzpmuekv.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3inudevip.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3uuogmqfc.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3psauoyuw.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3qqheurap.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3fcllzvdo.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3cslnvyxq.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3xsyixuzw.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3evblxrro.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3pvfbvcei.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3sqtbezhh.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3nghxlhnx.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3czdbvjzd.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3awzqprow.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3fuiouoat.html

esac
来源：http://www.52xcode.cn/Article/details/gt3bkqtpneo.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3ybyttcqx.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3fdkapchb.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3gupnfyzm.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3osqmmhwn.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3fhsddmfp.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3rfrffqyn.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3pygfcmox.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3qdpdlykj.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3hitfllvn.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3iwznqdaj.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3prtqwtpv.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3bixuvbfh.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3tglpeohg.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3eawjpuif.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3uaqoitwg.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3nuebwyae.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3rsxobqlh.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ousiebwk.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3aacowupd.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3uuwacbza.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3jjmaztvr.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3msykmfxz.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3zidchurp.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3vqyncnsd.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3vyxtonsk.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3wdjypzxl.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3pmtoygik.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3vhhijurk.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3ahllmkit.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3jloiprmk.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3mevruiyf.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3alksndle.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3nikmqpnz.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3stgxiabc.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3nsgisgru.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3upqqsars.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3oypyinan.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3nfppvdfm.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3nnrrylip.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ppwprvze.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3xkboiyfc.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3nrnudhsh.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3xcfcwgtt.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3ecdgthsm.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3pqwjwspn.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3rqojujrl.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3lfbkgtme.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3nerbbzfn.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3mubfrdjs.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3qqwaneoe.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3rojfepgj.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3hksubwru.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3awqagwsa.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3lbnivcxw.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3deklrdfv.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3tpblijjn.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3kdatbvvo.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3aykujdcd.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3rzqotwnt.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3lusjdswj.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3hyqfldck.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3uzxsojdc.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3wtjrbyqb.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3ofsysgkm.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3vrbuypnb.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3fgkblxrx.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3mqrwbomv.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3eudlythy.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3dlmnptyz.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3ybmwhknz.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3lptxpuwx.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jernuxcn.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3abcifmvx.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3kjimkvnj.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3iacfppbb.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3bqsgimbm.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3gaoecsmj.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3hsuwykzn.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3mpwoqqrw.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3vstniyvn.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3xktvkxpa.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jcsflspt.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3tvonfomh.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3umzhnzbb.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3irtwsfxs.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3ghehobag.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3dzygtvgf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3cghucrqu.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3ymdxodov.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3apashvjy.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3vugcxcpw.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3jgjlrpya.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3jdktxgrh.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3xfqepiin.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3dwpvjelr.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3hemfupcn.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3cjddpehn.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3qntzbqjn.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3glftighp.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3rsgwtglo.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3abvbkcea.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3dzrypbqa.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3dxfpcdov.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3avgnqacp.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3gkcdsyee.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3nmegktjc.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3auhipgbx.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3lpqqmjcg.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3uzbzglsr.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3orzvdqhd.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3ntqznyiw.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3smesaqoa.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3pmrycebo.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gghpjuvp.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3uhdbuwfd.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3vytxpwxw.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3yxwinyjh.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3vxufhnlu.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3lgdfwngs.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3dbdnwaaj.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3poowkxat.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3bnankqes.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3othrsqug.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3zvxkfbwh.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3mywmzzyu.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3sxxkorxl.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3copxcktl.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3svehywbr.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3odpbuvui.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3ppixdboj.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3ddfrvpen.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3qlscsfuq.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3buhvrkoz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3ilmxoeyt.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3adelcwbe.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3tplnkypd.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3pdlhewpb.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3sysxiyxb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dtzgacfw.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3lulmhchg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3onhxuody.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3itupepxn.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3icfggctm.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3xutioswk.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3uchwssgm.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3bonnxnpq.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3uzbgfwls.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3smayirpp.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3uzqbfrsd.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3fcrggakm.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3oojnkmjx.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3ejiksrjw.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3icbckbzq.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3tlnpazdj.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3erpdqnfi.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3myiuubwj.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3zyzykigs.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3qbshgdct.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3nwshknwg.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3yrvekypq.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3dbhobhhp.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3zuziqnhe.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3lqagfnmj.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3gyhbfzzg.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3bocggkxe.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3egmaalko.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3iuevrmic.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ituntper.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3medijhba.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3gdofvpfy.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3gpaqhmhz.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3tzlwoktq.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3xuaquehp.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3vhngwzxz.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3fknawuvp.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kjmzpnye.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wbvakhjt.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3ngjdzhtc.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3bbfvnpig.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3tqlldpcn.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3ilvqygvv.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3pafbslxl.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3reucukzs.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3pybwpvwr.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3zuotptax.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3fwcayqyn.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3pahywegy.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3kowaoncl.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3llncbisl.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3wjzrerty.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3wezphiga.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3dxazrfdc.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3jgiaenjw.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3pfzwphqq.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3mxnuvdrg.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3fevsicjl.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3detairzk.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3djfjknfe.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3jvqxetta.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3tjvmmbgo.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3oalbrnbn.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3gioprapr.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3jausrxsu.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3ckmryxbv.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3csnraocy.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3ayfxnoud.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3sdhtmqqt.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3slsvzess.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3scdhtqbw.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3vtlhwqoi.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3rvmgdprg.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3hwtutgms.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ndklcawm.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3mkrmerub.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3azrwysbo.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3latrapvg.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3buttkzyr.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3mhunxebh.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3bvchfrwx.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3vxstgjeg.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3skbmlsso.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3hobnwznh.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3uthsmrrb.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3kctecizu.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3urppwsyt.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3wffxsrcw.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dhloxmev.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3tcjfncvc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3lqrsqvzq.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3etrpytlg.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3enigjzna.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3wjyjltov.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3debtsxdf.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3detqjnmc.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3zzrrqhwm.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3vmehfgyl.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3xcsrmona.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3eebkqmgg.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3qsiwrxhs.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ogyybzdp.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3wkmotxre.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3pjsypcmc.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3ibkcxybv.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3xqtlidfa.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3jxkqtkkf.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3edejcncl.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3juvqbukx.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3dunbtbfx.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3angurbhq.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3tgwtyfkn.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3efabkstw.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3sgbundgr.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3zvrweeij.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3pgmnzdmi.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3jaddksji.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3zqczpskl.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3juocoffo.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3feffudpq.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3eqmwdmyi.html


<!-- 参考信息 -->