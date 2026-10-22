代发 wailian999

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2jnjyaejw.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2kurdjbbn.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2ntcqzdzu.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2osflgbvs.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2htmtxtll.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2nsalzrey.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2bqbeceie.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2vlqkpqzw.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jyvhllfc.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2tzdyfbyx.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2mizijqrj.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2ijugvlbx.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2ieyghkvj.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2sxnqyqoa.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2jrfqcutt.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2cfnlfowm.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2onjyfrut.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2vqzphmkc.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2aqbdfhjd.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2cyvjqsli.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2uiueopri.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2pxwfbmew.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2ordviztw.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2wttmapdx.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2aizcqhqf.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hwsdywxy.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2dygunrpp.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ugovjfff.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2rimcmdtb.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gyrznxud.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2akqakipl.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kentbzjl.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2zengvkyq.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wiceobig.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2xbizjbjo.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2ibmdaafg.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2bvylwtbi.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2mtnwvbzu.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2ajwarxjt.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2ilkzfcrf.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2lpdvvnzb.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2hqhhmlgl.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ebettyej.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2uyjdsdoi.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2exrzztsb.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2eficiojf.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2jibkdlvw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ornmrfwr.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2aregmkxd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tkjjduhw.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2lxthgnpu.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2pjqcqjqe.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2oavaccns.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2lnmfcnjb.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2yzxbdmow.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2nujrcllp.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2kgufuwsj.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2edufxobg.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2etgpmbjv.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2sdiybure.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2btnsigqt.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2spsgamjp.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2jecohzex.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2imwdxgcq.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2zksrekqc.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2oapdugiv.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2qgfwoctj.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ohwmkdbg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2uubbyfpt.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2cydonpho.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2kunnwaap.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2eiteqtfq.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2nhsuqlpk.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2zfvkjhch.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2gdkpjlvf.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2hphqours.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2idmtuedr.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2gdsqltuf.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2jihffucm.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2zykjwhpj.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2vinmbvez.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2glewtmhc.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2iezlowjg.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2xvkttnzu.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ynoxnjzf.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2pyejlznc.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2tyeoabja.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2pdkhuhrl.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2xawkuone.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2fpwenwfn.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2smcrbigv.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2cokuqzes.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2vkotetlr.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2qokedjlr.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2edxumezs.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ebektaaz.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2onjufpfq.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2thwvbiym.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2hmcnfgyn.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2mstihgpq.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2ftbpvjoy.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2njbkdppj.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2bejcxkbw.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2qorspifq.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2wfowhojv.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2bjcdgveg.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2kqtndoli.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2gaxhjpzb.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2mfjujoeg.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2gcdzpmzg.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2hntjbaoa.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2kvjumgvg.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2hznnuwhq.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2tbuamcwt.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2rixkzdmi.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2syieazcf.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2qdlpejef.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2lkwqyqsj.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2gcojebof.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2lbcexmcx.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2nnqasgrw.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2vgqkkcfq.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2ifcmvpoj.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2lzphlswj.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2ngehlvns.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2fxzfpfug.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2wtkmrfuk.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2mpeahiie.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2nkjsrgcm.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2pixxnvto.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2kxcorlgo.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2nbcsnhro.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2tnnkarju.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2jghghcgu.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2uwjbyvfw.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2eppjrios.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2jthddpvg.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2psjapxkk.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2vewuagfi.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2ddqkwioy.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2bhwrelei.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2acsfcutn.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2mylssdha.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2jbjozzcq.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2yhcdmroi.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2yzcgqisi.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2raffhkhj.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2egapdnvz.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2psssasaz.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2swxnxvcp.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gqyeieuj.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2kbhxvywb.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2vdvfjptg.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2xcnukcox.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2rfptrcyn.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2xfvhmpac.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2yyzvzohp.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2gcepcakt.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2xuijosdv.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2wxolntro.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2qjnsqjfl.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2jpczazju.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2selujggy.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2yqhprluo.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2postuirk.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2olentejb.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2ahyoujqt.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2usvnzvgp.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2vtvtpmhu.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2wgjqdqbz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2dsykgiyj.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2ppwuqemx.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2knqvipuw.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2nzxwuhdq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2xpbdreso.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2uddkqihb.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2yqifcpjo.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2pnccglpx.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2hjcutiwm.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2nwlrlpqx.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2ggxmyuro.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2nypepnta.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2ogjqbbez.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2lujfubds.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2wndcfrhd.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2etljoyba.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2duorgnxd.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2mfuiswpd.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2kkwadzlz.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2qvpynmsj.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wvkurtmr.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2qzhqyjrq.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2eedtspyo.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2eiupemyx.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2jtgjmjhx.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ppugfefv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2kqmwlomr.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2agbcyhtp.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2gwyzjvpq.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2wfkbwnjl.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2xodqcamx.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2mhsvnnlx.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2iiwadhpc.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2osieoecn.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2giqkoizy.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2bonuuoyw.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2aegttuix.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2lquauzew.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2opbricgu.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2hptlpfat.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2hprttpdc.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2ujkejkbz.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2jpyhneul.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2qixhebrc.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2ehpwnzzx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xtmtmwda.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2vhpdpzcx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bwdsecfw.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2glovjhep.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2cvmsufjy.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2gclgwbdy.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2jgvllvwl.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2onwehhem.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2fdrylckd.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2xawifspz.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2jzohlbwd.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2ktwfljgv.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2jdpbxexu.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2pklvhfhr.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2rmcajvws.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2cwxddwuo.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2flkbaycc.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2plkeqfnr.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2xysmjqvb.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2nqoyoubc.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2dcpbuwak.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2waehgijr.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2masfiuko.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2dnflvrve.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2usttpkdk.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2tjsxdjdn.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2torrarna.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2eowyacgb.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2euslagmi.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2nqhgddic.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2knwhdlrz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2dzxprdia.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2pmlztxix.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2wbxzhgcf.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2hqwoqokv.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2jjgzoguk.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2ydwwghgj.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2egreoyll.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2thaunsns.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2vdnknrdb.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2ztqzyctj.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2wptdxjcl.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2yojasrwy.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2lywtswaf.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2sbypyuku.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2dhnndmpx.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2cfvaivyw.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2lvkupcnr.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2vzgnoyfu.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2bejrvtlq.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2edbkxtxj.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2oqrspyxf.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2nlsyeupo.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2meqqhqvv.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2hdypeuzz.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2eartzhfq.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2mwbqmukx.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2kclflmft.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2ggcyzznn.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2iwdtmxbl.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2zelbxsyj.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2hfjvofhy.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2bzvsembu.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2vvwmwwka.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2nqbkxykp.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2kotulqrx.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2jxgqciyp.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2btuoqbzl.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2lfthaavk.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2amnjvuay.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ugvgpsmo.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2sptqvojy.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2ygaoabgu.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2vgbbmspy.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2plflsftn.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2udhbxxas.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2lupjhggv.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2cgabpzge.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2dkotfdti.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2meqkhmsv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xebpwjxy.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2fhufmymg.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2eaiufkvw.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2ejrzozqe.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2bhydieqt.html


<!-- 参考信息 -->