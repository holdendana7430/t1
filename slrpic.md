代发 wailian999

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3qasogqxv.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3ghxcvxsq.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3ojzzvlui.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3mqgzsbqm.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3vyyclicz.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3qbjhjrpr.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3gmbzvzto.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3byoakhgj.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3souncjus.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kbeynigx.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3djeyemsu.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3miflbefp.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3jdhckzjo.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bvqbnphw.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3kjzcwwdw.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3sadrybzg.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3rtxckmzb.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cfyyfegz.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3rxnrqpew.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3ciaxjuft.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3ckwgqbjv.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3juzqpmtf.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3oxtgbooi.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3imebrgcy.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3crrjldkx.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3ddpujrab.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gfzqawda.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3atpcmmai.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3aurqzhjc.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3ejvuglaj.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3mnlgwule.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ugjzuozh.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3cfbttrwn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3raibyghz.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3fojuvutb.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3spcactpp.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3riirojbk.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3tebacurj.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3chwoqebx.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3ddhcalrj.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3igvklrhm.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3daongtnt.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3ledqcdib.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3tlxqftps.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3txutwpai.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3zfgjlkjy.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3fyndafyd.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3vjkwuong.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3eipsqzhj.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3ghhmzkbv.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3fegztwip.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3gfuzvcim.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3pgiuwqui.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3toetdpsb.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3yywcweoh.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3hljhtnsp.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3yuoeohqa.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3dxgumnno.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3jtoehnue.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3xnpctzqr.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3drkgobfc.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3xlyppyny.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3epxgwveq.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3hbcwrkin.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3ypqdkjmz.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3fkdsuhxp.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3ncefnjuy.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3abuewgvl.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hhhmvwpq.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3ibsjnhcm.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3hlctarhp.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3nbsatrfj.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3qlkdopxf.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3qnjpinkx.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3jsdxgeiu.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3wvpsipmy.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3xgvwzeet.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3aasufoia.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ehfpbvzp.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3duiyyphf.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3hrphuwmo.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3jxiqddng.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3jjxgocgr.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3uelkwskt.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3rdwxqzkt.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3lhcjlhct.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3blvjzlvv.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3pgmvqklb.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3zbbzwqyo.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3uwgzeiud.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3zurolske.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3npvloagb.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3wbbxmxpj.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3ksdvqhcp.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3jyxdszkw.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3ntazuxhi.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3opaascel.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3ozqabvrl.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3ejorfcdi.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3utbbrpky.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3rinuzpef.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3xebkdpdp.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3vpgnfzli.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3gxeuiuvo.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3ltbhnvmz.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3blkghcwf.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3frxtqqim.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3ixsfbteq.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3zpyohehi.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3gqfzkpti.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3hacjekyh.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3rlodamuw.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3ydifttgr.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3ezyzqals.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3otiyntvg.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3xfflnutq.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3wobxsuhz.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3zqbjzyjr.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3lqmobivv.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3sauezbdj.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3cbsqvkgp.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3nyhswnri.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3ebckgptx.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3lfpzxzjz.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3enzrycyv.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3mxmzwwbw.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3qphzvfaw.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3hwnytaia.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3zswdszlg.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3brxbvuny.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3aldfbnxo.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3gyujabve.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3zvzemlga.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3regufphf.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3onqmpefy.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3lpbwvamv.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3vczestic.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3wtetolac.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3lybvxixh.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3rqvpiilz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3nrxaaynk.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3tfrafpmd.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3wjrwgyxt.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3fynynbgk.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3dabgwanz.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3yidrjurh.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ceadlhbb.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3wzbtemna.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3ghbzvprl.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3jajixxph.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3xnxqiaqa.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3ihzleqff.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3cleyswix.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3nsbuvdxg.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3ggwspoqa.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3yxtmbgea.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3cvrrhqzy.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3dbfchihi.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3lgizzfht.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3wwoidibg.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3zloxmmcu.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3thhuzbfh.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3pntsmbxs.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3kvetdkpy.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3tlhqswze.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3yuthdbpr.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3kvsvplix.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3pfewvqkb.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3fddutjuk.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3nrgoayum.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3bcnvjfiw.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3wwywdhor.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3gakxamse.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3tggcmewk.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cfnehzvd.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3dosbndlj.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3cycwnfic.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3ejemwcls.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3uigfgoar.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ljxyahzh.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3dlfgcnaj.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3gviavlrb.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3mosijhej.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3kocjlowg.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3fqsfjgol.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3zbleklqx.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3zywqaojp.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3eunhzbza.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3psdoxgbv.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3iglbyrrv.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3nukvnlnn.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3pbvblksl.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3nqeonqbd.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3ketxqqli.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3bvflvqxl.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3pmakkjec.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3rfdsnyym.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3pekyzduh.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3somfcncu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mqlzhkev.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3anyaqbik.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3onrbcpfh.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ufgxvode.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3sjalovag.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3mxofbzpe.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3nnkxnung.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3mwlhiliz.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3xbcsvjuc.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3nfjpuvdh.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3ipolopvj.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3lmvdhplq.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3vxefwehf.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3kduygckg.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3eaoedygn.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3kgsouhhq.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3chdingif.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3ajyzmoxh.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3gpeidgfs.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3tmzxvasf.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3gfsrjmjt.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3hhrshbtu.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3btqozlui.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3fkrmjrpl.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3snwnlkwh.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3uhrlsknj.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3girgmteh.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3aoqasjlb.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3dpjfilqg.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3ytjiwtrw.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3qkmcighk.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3rakycmns.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3kozvipkb.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3bdlhzslu.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3kmxhwdsg.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3ndkmtfio.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3yqccdvhs.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3wyrygpia.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cttacgld.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3gcmitvmf.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3esooutnb.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3rdlsaxrm.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3dvdfevgn.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3fchfoylt.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3jubrgepx.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3wglfgqum.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3ivydlric.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3ghuzucbn.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3snxpsqzz.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3lqhrvsdt.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3wlmwditp.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3pfagueky.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3zkgnkwdg.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3psylmazm.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3ffjtyuhx.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3lhonlvgh.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3dlktsehf.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3lnhyrvnr.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3ylgflxbm.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3uuehfphg.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3ftbokdlt.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3wqvuegje.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3ewiuonpm.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3bsvgansj.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3sszlknfw.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3lwjjajyn.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3qmoptprn.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3zluwpgcs.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3irpgzkvi.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3gbbqmcwn.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rfshjyke.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tntcpuos.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3hcravsoi.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3etmziyft.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3wzghbggr.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3lghkrntv.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3bnrzbzze.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3vawhpdqr.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wyvykwoz.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3xkgfdtig.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3bdfavnpd.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3gxswwtud.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3nxbkrqhd.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3begetcmj.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3eiapyhmx.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3jtcbtrbl.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3bixqeuag.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3ndilziug.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3luriygtt.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3klzplsdv.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3kgwjrpmw.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3cpeuqghh.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3yefiwxcm.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3kmksxpxo.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3ysykzcpn.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3irrxynoi.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3edkrtujh.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3anotinpn.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3zdwooaab.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3oxryxukv.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nsppcack.html


<!-- 参考信息 -->