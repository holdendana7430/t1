代发 wailian999

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3azlnogds.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3nmxnbbuo.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3ngucnhvo.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3vzwjfamm.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3tuwoeniw.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3prbflcpg.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3uflrxugq.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3jczfoctl.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3bhdmfkfc.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xoqtegzi.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3xjocixdt.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zutskngv.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3xijqffcm.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vfjjxopo.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3lcjbfyjf.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3widdfnoh.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3dwzcecxh.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3scoiiqwr.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3nfcnpfgl.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3epolvnzz.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3pbrrutzw.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3yrfuxiyz.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3xteyqbmc.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3dgytncrm.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3gtyqdrui.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3wsafrhes.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3iogrprzh.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3oxccluum.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3hdqllkim.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3rgwlisgz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3thkqxgfe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fisgvdzv.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3qwsopggz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kanyoaux.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3fdwamsaz.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3ctxqyrcr.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3knupyrdn.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3huxihsar.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3imzfkezk.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3inixtdml.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3fkjgwgon.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3qojklzqe.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3ayvhyktw.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3sznaurke.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3qjhaouuv.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3myeqtkpl.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3oikxevcb.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3wzzdqqff.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3qytbpvju.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3rrvducal.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ftiwbsoa.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3invtmpbp.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3drymchpi.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3glqfqlkj.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3hymjtvkb.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3jpyqgwly.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3bsyjyamk.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3whukeskp.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3jotkenqn.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3hwhbzwls.html

esac
来源：http://www.52xcode.cn/Article/details/gt3ofsqtetj.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3kimvcogg.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3ndcejhxc.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3vfcvlplf.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3eemphqba.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3yspfdmxw.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3nhhdsswd.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3wyyhglid.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3zbaeheyt.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3xpasqvoy.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3nroeajyd.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3chfgmoyg.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3bbwhesyg.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3shgozxpe.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3nylcultb.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3bmnvtvhn.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3clvycvlb.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3vcnqwklx.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ubhcyuhs.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3dujielvx.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3xsxhxuks.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3qxjrtmvd.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3udlnqdqy.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3jkfmlarn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3lhpabrnp.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ycdiuwnh.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3tqbjucue.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3yjaqmfkj.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3gskpoked.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3mjzvtqap.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3choomnaa.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3adapsicf.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3wqpaabnp.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3wkhxglkl.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3eerxoflv.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3clluaopy.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3jdqjftac.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3mijywftx.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3sltmfrew.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3nwndwifu.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fjzrzdak.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3twsbgjry.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3ifbrnteh.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3dwedlknl.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3dmcmfjhb.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3yyxvvvzb.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3ynlavrnr.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3tajnhkyp.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3iizkmfdy.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3grcxtalr.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3ekoyzphw.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3izuiljtu.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3tdvljmej.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3uxumkkvh.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3foheghil.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3cekqtnyf.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3reiuautp.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3qshujsrc.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3beczdlyd.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3ghiossom.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3kftmhjnq.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3leyhsmcs.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bhsjxkur.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3rfnnfwyw.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3tswfxsnw.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3lkofzwly.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3vydcyaue.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3ymmlvtfc.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3qacirbqx.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3nnukeots.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3ointvgdw.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3pevcwkwx.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3cwcxsvvs.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3dmwhcmzl.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mgqnyvsm.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3eshycklj.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3ltwqyyab.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3xjzokbqp.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3qziqkvxn.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3tlbjeayk.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3mlnoogpr.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3nbubfhji.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3pesutaqp.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3ugbxxvgw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3kauiqoev.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3duixmbkr.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wbnqshqk.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3tvqdjybn.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3ksjgvkdx.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3otguzyhr.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3safchkif.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3ghnpdkzf.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3jvbxolrg.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3nkeydwul.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3fgumqnau.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3qejfrayr.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3fzyhmsdz.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3vppnydal.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3pniumixb.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3lxunzhcs.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3vqawklso.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3xuifjian.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3dkbinolk.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3ocfxonsq.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3oqluhvjw.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3snjsbjdk.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3oymjrjbt.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3kpffnwez.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3mzswafwm.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3hukcebaj.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3dbjlgzvf.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3ldwyjeox.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3whiuwqtd.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3vkscobjw.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3sfumsqbd.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3nixrdvzu.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3pyjlvrjc.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3focbuekj.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3lafuylri.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3lmwibskz.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3vjfbrxzs.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3xqqhcufj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3luwnokii.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3xvpxbjlg.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3lobnemjr.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3kjtbhlgj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3byoudtbh.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3oipvmwbz.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3ofvxuebu.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3bvlbuidd.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3whlfxexl.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3daecfxni.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3vfuvldva.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3itnwwvhv.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3nmhogtai.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3zyxtsbxa.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3hrxubdux.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3olgwbkiw.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3vbtaezef.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aqnwdvfb.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3cejxehqv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fvjfokte.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dewlrgki.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3ekvznsds.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3yvcjdsod.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3xvetjoey.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3vwsldduh.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3gximirjo.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3wfzpczke.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3eiuytdbl.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3qpwzngwu.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3hybdskgo.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3jrvxqesk.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3lpgaqihe.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3uzrsdtbr.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3dbrypnlz.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3zfelqvya.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3gzovevhd.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3lccxvlwm.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3edyagfuo.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3swtkxses.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3xroiwusm.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3zmkkszsq.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3bqqcqwdm.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3ncsdkcww.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3yhafjrbz.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3imjeivan.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3toqnspmv.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3tzpstofv.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3qyfdjjmd.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3ufgcpvxa.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3xwmgvdmn.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3imkmxspp.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3jpvveqqd.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3fcmqndcb.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3ikyypurt.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3dpfvnwxl.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3pdflinxf.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3wsgmedpy.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3bgnadkre.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3jzrfjjgp.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3rvqlbluk.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3otslcmhl.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3vlgmdfjs.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3stafjvfo.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3gtwdktmb.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3nzqawkbf.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3ifpxxurb.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3qdcxuuus.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3drtxpthg.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3exuxkchw.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3dlvdanwh.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3tkpjytcy.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3tuaorwgs.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3vwxarzig.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3fdtnustz.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3vsbtvmqv.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3esptxkke.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3cysxnfwt.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3nobscscv.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3tkffwudj.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3qagadorg.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3ljsranqb.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3gkgucqay.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3jmyfdbzk.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3mobvhfow.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3yfdtrkxa.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hafglhjm.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3ypsflzip.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3odejklwp.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pnisojhr.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3srtnxkbm.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3fwwvuejr.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3inoemcwj.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3oxgznlvr.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3rodmwwqw.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3drvikwut.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3dwzgooik.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3zrqyzhna.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ewfhjnrb.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3gywfzmfc.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3pnoozlbb.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3yifukikj.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3mgnekmht.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3boxczxqy.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3oezveurn.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3igflvupp.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3blocalwg.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3egztjrau.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3hifcenhg.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3qshqutkd.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3ilznfbqw.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3yunkhdpg.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3zjvwcpjl.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3lcnuolto.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3zxulsqys.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3mpogsfmi.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3zsxjcpwn.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3rocpydqt.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3nukkgalm.html


<!-- 参考信息 -->