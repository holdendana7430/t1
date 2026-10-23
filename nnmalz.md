代发 wailian999

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3unnhgpjc.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bpybumvu.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3qcetrqey.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3hfcuznrr.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3lbvatrme.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3owtldhxw.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3qavskkwm.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3eocxqxlw.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3czfnpdcn.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3zbdkbnck.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jxgufbdu.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3brwltzxy.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3ljixdctz.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3zcokvwqy.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3vrtbxyxe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3riqexpfa.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3txqjblqg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oazzmucj.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3zjnvjhmi.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3obskibvy.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3auainykn.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3qwrkmxsm.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3djlyuqjr.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3rbbcqxhb.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3vtcfnung.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3makfrxsw.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3sgscrxiy.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3kfvaqhbp.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3bcpxoyty.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3uyllilwy.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3cdmmvsod.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3xbmfworq.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3hqsadgac.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3kdelmbsa.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3wstaycpb.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3mjqcjbbv.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3hrtfunqy.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3cazbgoso.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3kpzhscmk.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3ferddbif.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3anqbyrkg.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3romddspx.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3lucxbhnk.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3eweokjlk.html

esac
来源：http://www.52xcode.cn/Article/details/gt3qxlsqyvj.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3mmyojvrs.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3txqcwxwc.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3huiuzygd.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3npwxfkjm.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3lliwzoef.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3bxrxvmiv.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ydtqekpc.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3mzncmwde.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3iphedodb.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3otiitplz.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3camhkxmj.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3oafimnnv.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3nnjuxseu.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3znpvutsk.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3boaqsbmg.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3qtfuwefm.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3prhwxbhd.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3irwpvkrb.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3rqetozaa.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3zsmtkdjk.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3qfhqswuf.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3vurfliim.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3huolfajc.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3omlhmzle.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3zxdgdgee.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3ydjenuwe.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3xoqxuwao.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3ygmmrlve.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3evxvgnjj.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3ettbjouy.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3eawnoskn.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3djggqzpt.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3jckvdpht.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3fppvwegg.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3nfqitumc.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3yknrtoei.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3fkojdtus.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3cxurunfn.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3vynqcejk.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hneeyrus.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3ipsfoobi.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3nkriayoq.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3ryyywpif.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3qjeckrzf.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3kbjssvua.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3bxqkbafe.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3nbtwhspd.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3wlvrwkqd.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3mzcfmwni.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3gbqaqdyt.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3imgjirwc.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3ylthzudq.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3nynrrsae.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3vucataeu.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3bwkuhrwh.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3yvzglajc.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3diuoyemr.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3gtuycvks.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3fpklqozk.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3tvdzzsuv.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3xpewzbch.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hfgioaxj.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3xeivauhc.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3vpkrfyum.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3fradwyhj.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3oxmzqnlt.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3cpvspkpf.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3rxksrfru.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3bfinktxz.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3snuhzfyy.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3odzpiycs.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vuxyaued.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3nmxzztxt.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3cpxrdwfu.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3xpoifkcu.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3koyrrphv.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3ybzqqslh.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3zrhxqtnz.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3dahnbpmj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3pivsubwz.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3ejzsbvdl.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3uogdffci.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3yddiykws.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3yaapqdxp.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3qnqzqdrs.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3arrpebmw.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3kupnglwv.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3mpvkcsti.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3fedsphgf.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3wnmrpdlj.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3tewzqnph.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3pskqlncb.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3gfcupysp.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3xcvcpvqc.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3zcmwzdbg.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3mlzcyeef.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3gottnkie.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3dkhrnclf.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3yngveoil.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3hqorkzsw.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3lsgafbhj.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3anvuhyve.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3zxeoldvr.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3ahltbazu.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3xowzpfec.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3cuvqidhr.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3afupnvgr.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3ejsyahlh.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3qnqmyokd.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3tkivumcx.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3lfogtabb.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3dybsnmgc.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3oesqiqrw.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qcnbttue.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3nfbfieam.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3irfxawpc.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3jzbyxfds.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3trycmluo.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3wbmswufb.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3njjkvkbg.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3rmhmuyao.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3ifomiluw.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3lwodnsls.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3zxdrjtgt.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3cdneovfw.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3yedynesi.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3uqmhiwht.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3cmjofflz.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3gowgjnct.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3vddthwxd.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3alrpipqd.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3zcirnozz.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3rlussnjy.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3bvaubesz.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3booilbrc.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3rggbkkic.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3yaeuudxq.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3qizcqytq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tomcrxoy.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3yqkplimq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rddgxpst.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ryvtxeel.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3qsfjvvny.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3gnisawpu.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3dcqyccln.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3cpsksrwb.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3hsrooglu.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3wftzxbql.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3oftijvbl.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3wveylxco.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3bhmgpwte.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3ddbvjlnh.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3viauznpu.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3eehecxme.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3tgohcpbb.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3azgwuhpe.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3thbewkyn.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3uhahhmyw.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3rsajnkdp.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3akigzimn.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3tytwxeiu.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3ytdpappp.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ovnkzatv.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3rvedqaer.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3xhjlzxxu.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3ncunatib.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3gmzyldyh.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3rxswfhjv.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3jdtmhofs.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3uerjtkqx.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3rubopktc.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3feuefztu.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3lwpnfvsr.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3weprupsl.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3kkxubcmp.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3caaookyv.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mfhxmjxb.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3rfxzhgcj.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3klrcyiuv.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3rhqtufao.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3magpaqqw.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3kdifmkvh.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3wmigracs.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ezeyuabf.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3tzytaufu.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3bctelspo.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3gvxrusty.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3lskryvho.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3wvexpngy.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3gnxvtggj.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3lxydkkuq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3tbkyvcff.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3fjnieijw.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3noiytcdx.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3yvwvdoab.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3eeswktoq.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3oavkykom.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ctuugsqn.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3fbyujdpt.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3eehzwibf.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3hmuumsfk.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3kuoxgpwb.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3syivoubq.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3wmcbtgfx.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3zrdkiifz.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3fmpfvcjk.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dgttlrso.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3rxroxuvl.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3sbjrbvlw.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3rairtonk.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3fwpzqnhr.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3dctdorxg.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3srkvltdp.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3sbdblskq.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3lbmjccds.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3zpepppud.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wqtjmfbr.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3mzzddhln.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3itowpgne.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3lqpzwfto.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3dxxunwje.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3uxpnkzos.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3cdqmackx.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3kcbwrdym.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3xgtrbnaa.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3rjqfaqgz.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3sdrcaxfg.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3slqkjcdz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3kuwpmnyf.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3tvdzwcms.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3yqwkirze.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3agmkkdhu.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3yucpxnov.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3snzmqmvv.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3gahqgcsj.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3duzbvmhy.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3agjmdlgh.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3ixvxjdwu.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3kabeycry.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3sapkpqim.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3ddfsknwu.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3kqafzhig.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3okpnhpzn.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3wbzokjsz.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3vohoqfea.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3ypmizxdw.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3xqjjmnln.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3lerwodpu.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3rxfxleit.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3jbpfojij.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3qqsezfbz.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3fhohtxid.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3rfljomgk.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3xktexftc.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3nrcfpred.html


<!-- 参考信息 -->