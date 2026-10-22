代发 wailian999

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2rfnuxjlm.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2vatocndp.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2yuaflzhq.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2fytpatvj.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2qmhyvacr.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2jewhskvp.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2mjswutap.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2ybhzlvzc.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2djdohriq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zwycimif.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2imosorza.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2poiypmcc.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2eblhcifw.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jewgbvqu.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2gkakkbxw.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2chkichri.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2yzqbkqlm.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ciaqhpnp.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2nidjixay.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2dxdqatjj.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2fwlxetur.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2sjuvrfyh.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2prndjrqa.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2rgonxgkn.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2pbcgfspn.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2hfpookqr.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zoeagshz.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2nofluiit.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2fahyhowi.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2yfxhnrrj.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2pfjclflt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ltickhkw.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2txngsmis.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aelyxiwy.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2gdotqikk.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2fmdjttgl.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2wusxeoet.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2fmdflwjq.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2hcqesjjs.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2gsjpntyp.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2ulgkjoch.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2fdudbija.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2dzgdjsxs.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2tduklmtg.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2zsmjtphp.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ahaddjku.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2vhoxkzkr.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2bjumjfpq.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2rfjllmhs.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2yboevanx.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2jmmmmsua.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2rokocyfy.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2awqwxovl.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2ebfztvlv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2aogtlkda.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2tmrfidbf.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2gnukhboc.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2khqpnnto.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2roqeqnoa.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2pztqowmo.html

esac
来源：http://www.52xcode.cn/Article/details/gt2eyyjyuzm.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2udsudjcm.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2wyexzqet.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2kgliwkdi.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2szdmmouq.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2nabrrqkr.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2zmjnovgj.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2nbjxsheq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2jdtthfpk.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2aunnxovo.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2sglptviy.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2ipcbnewd.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2opbrxdwe.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2avlaupbp.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2wigjtryv.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2tnosozld.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2wvwpyrwr.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2zuqatmri.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2dypmckef.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2kwreibqo.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2pfpvjthl.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2fqlcaipn.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2smfadlgg.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2hbzckagi.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2jvttydze.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2ugxgfati.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2dgwatlhd.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2oykcqyga.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2nokgqobk.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2tkopynqk.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2wgqbjjtc.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2shifvdcz.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2krfuzwfg.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2xplrknun.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2oenvbuqz.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2wjsjdqzi.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2rsxdscnv.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2ujfqmvnn.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2hzbhkxld.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2uptnxqum.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2klwusrwu.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2yjxbdhib.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2bgygcuei.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2brkbbuyv.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2thxayegy.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2gihcfkql.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2grutbwtl.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2ahenlgvy.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2iotiggyf.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2skasywsw.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2ybqyetzn.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2hnchoerk.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2aktnnonu.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2pumzwkyg.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2khschphj.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2fedhvbuc.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2vhqhzppn.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2atxbtipf.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2clsuokpf.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2ldjbrptk.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2rkqynfyn.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2mhasdhpi.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2yjkxtafd.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2depkhvsf.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2dcjsyiam.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2vwogelbo.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2zdhsiawi.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2swamqbpz.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2hhjvaicm.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2ragwjiyy.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2kkijevny.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2vowtvbzm.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2uimvqfle.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2hwxelepb.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2botoyqzb.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2iywnxczx.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2slkxrmvf.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2rstohdwl.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2oqvabwwi.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2itnyiici.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2glzpwklc.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2sunebnjr.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qqpraglj.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2zrgmaaoi.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2rcralxwe.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2jwvfschg.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dyzywvab.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2xvwltbkb.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2tzlhimmt.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2qzflrbxq.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2lgduqipo.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2mzlihbhm.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2gtjlrlhm.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2nknwpybq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2gyjobthd.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2zivlcvau.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2oqwrpcmm.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2arhedlwd.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2ectwrueq.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2hoveralc.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2hvkbuagl.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2zdklicuq.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2wmpndgjy.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2uoazsxky.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2byfhjnel.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2iptsgntx.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2iltouaga.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2dvhqgqes.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2tgslcwbk.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2xaxynjit.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2lxnhqrvf.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2rtghslcr.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2smivyyxf.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2kheqbswp.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2shwzaawr.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2saxwzixm.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2hcnhmzec.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2dejkighd.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2qmchkrxk.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2qadxzamb.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2ydpaqbvc.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2simnlhhk.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2iobaiftv.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2xsgwxmpe.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2dlvpttvx.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2evtlotch.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2ulmoiapk.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2btptzane.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2ibuwzgfz.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2kgzsbswd.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2vepnjatl.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2timmncot.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2gwhrknup.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2ldlyndhf.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2yufxejrr.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2tsvnixae.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2ycqlvfja.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2xpdnfuwl.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2ubaqldze.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fdnqeaak.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2jthynntu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2owrmioav.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zpsobhpz.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2rwoydjry.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2qgkfedhn.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2urtvowqo.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2rdlcrssv.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2wlfgwssc.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2qjnnzgin.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2qhblwczy.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ckzxgnpy.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2cbhaubfe.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2ubmgfiix.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2dyjrmopt.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2lantchtf.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2eknypgfc.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2qabectfi.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2mtrewluh.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2agtxoydc.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2mullbinn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2xzkwndbg.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2ynrdiwjr.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2icuoalea.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2vsaisjgq.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2rwxwmaxj.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2daxyhmfh.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2mjwbulir.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2cmtnnbws.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2teakfvwt.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2qrjvdcsu.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2ehryopmx.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2qfetvimi.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2pjuveiuf.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2jxejcavd.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2isrusomw.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2dytqmayl.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2bhagdcql.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hwwrqkrk.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2hggbpvij.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2ugftzduc.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2nqxrmeny.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2ktnzdudi.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2lrkqyxdh.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2djmyofgl.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2rfqqffjf.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2ntykesek.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2cyazaqop.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2rtbkgwnu.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2knsabzpn.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2mlkcxxhs.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2aqrqpoen.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2eqkieeid.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2qvkhwhcs.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2vmujzsyy.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2mjcvvift.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2xybetfsv.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2kzcwprip.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2sfmwwzkm.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2soiedgvc.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2vyttnoba.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2eouqexvp.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2grxltyuy.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2pzxhkftd.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2nlxuvccb.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2ywuxdeer.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2akjvxcxr.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2qpeufbex.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2lriolzcw.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2qubhmxtw.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pdyrsrjh.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mgtfrykm.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2oznvggbw.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2dwbosoow.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2pdedjyef.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2lzhoqvlk.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2awpsowxe.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2uixjbpca.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2oxzullyo.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2nskiuugl.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ulzqzxer.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2ycmnauln.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xemsfrnj.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2vgmtvuyv.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2cktwbxmf.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2ouurmxoz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2nkvdialb.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2idakrlmt.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2uebrkoul.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2gjnrbbhm.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2fxnoyzmi.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2cidegppn.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2xjhsmomn.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2zzbnbztl.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2oggvozpg.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2tsdzbbhh.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2rfzpexvj.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2lzbklhwx.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2xgxnllat.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2sgnexooj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2akvcomlh.html


<!-- 参考信息 -->