代发 wailian999

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2lhrzpuza.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2rylhjpcj.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2phmdlklr.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2ruprfini.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2nojlxbcm.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2mjvsrojn.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2mfvfgyoe.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2rvnmfujl.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2nmrlzhub.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2jrrwomms.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2jwrgbgcc.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2zcsrxyix.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2roeapsyf.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2sgwdjnpe.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2jcbinmni.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2dxfgrksg.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2zjsqtzln.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2dqrybcmr.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2vhtplvss.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2ytleizkb.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wepcvhfw.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2uiqfkioo.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2pbfgaphx.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2fsrmcwjd.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2jgjcrfkr.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2hvseifpe.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2hdonivlt.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2hmybxxxe.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2jijdxeop.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2uhxvtmsx.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2lemgdvou.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2ftfxlqzx.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2vgilprwe.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2ehivnrnw.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2nrurlkxs.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2vghwnyzh.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2gywrnkum.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cyzfvbvw.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2chvzklme.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hdjgsros.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2vwplhcjb.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pwjqoxye.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2iqoytvom.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kzqbnwqz.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2ifhfkbtl.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dggjvuib.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2apcdfnrf.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2eguifotm.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2mkfstjew.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2bhmrcleg.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2enkkxyrw.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2kqrdkurf.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2sccmkpbv.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2yukpahwj.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2eudrijps.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2fylyabxw.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2azzzwnwh.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2yweekpyg.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2dxirnmvm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ogayqdti.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2istlirta.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2znhgcegh.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2ocoilhgw.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2qnewnjsi.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2zufpaszy.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2ncvaqdih.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2uhukkomt.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2uvcokmpy.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2nxeydwtu.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2iiewwlbw.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2iqzpddzg.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2aezsaywk.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2pehbtsye.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2tmlcvajb.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2qugnnlrb.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2ofmjqjsg.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2bveocfvl.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2tgyaxdmu.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2ofxglnhm.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2dbfurwww.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2pmtgxgwf.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2jlxnmphy.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ucizbtqf.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2fxzioppt.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2gtzivzyf.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2zeuojhdc.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2rfbfkrll.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2sjsjcjpc.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2eygizzpl.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2sgbuccdn.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2vxgiklml.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2zaewmmyd.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2tpizgppn.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2tucosfcs.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2vhcmuldf.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ojsmhyfx.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kngopeoc.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2pjxzgyqm.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2geunqmzb.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2qvsymsyu.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ghbujdqt.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2xjyjvlyr.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2yyltffmk.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2oxafaath.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2kqufljzx.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2jzqizwad.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2bcgxizet.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2zicmfiqc.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2tdhfzxmd.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2tmvrctvi.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2crsxlxzw.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2rkuvuevb.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2ndwpusqk.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2nysxwwcg.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2dbkexrfa.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2tekdcnib.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2ihmryddf.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2iputydmx.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2ggoupxyj.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2omdicwaf.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2yvmzyslp.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2ryoxdyep.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2kwhobilh.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2lxqiusuw.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2fxromryg.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2phmxsyuo.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2xptftzdk.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2mvdvxeuz.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2uxrleldi.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2rmscerjc.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2tzdiusba.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2wolsimso.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2qxxuhios.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2tklronbe.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2mtrutrou.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2vjmjsakj.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2uxlfzqdj.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2dekbdbsj.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2aswwcmej.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2fitqdavu.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2mnjciiey.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2iitqxcwp.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2tdwdtegx.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2xknszepv.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2vvlcvmrs.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2ciwqucya.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2poticqaw.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2pooaqvpl.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2tjpavrfy.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2zsedajix.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ramltvcx.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2bsvfbvha.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2qhgbblgp.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2stjbmasg.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2wqfjpfbs.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2dvbgbfwe.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2dhetmujw.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2feapqxbk.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2jkgmckou.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2hwggptog.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wwbsjxne.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2pnuitghe.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wnlzzcew.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2lsvyabrv.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2mhxtosmb.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2nmbnkadt.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2qoykirkz.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2jyngwfsh.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2cyfguefa.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2cuxzuiae.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2njkjnkyx.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2znkyqdjf.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2ysxvznhz.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2ejwzhepp.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2kfycynnk.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2xhooiydz.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2rbgrfmlx.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2nnhsqroa.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2fqtscmpw.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2ijcdsusr.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2kvrqnyyi.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2wvjysman.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2slodtkms.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2jlttacqi.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2lquyowzk.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2ijpewmzj.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2nqcvjwmg.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2iyybshvy.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2efyfjhxc.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2tcnzbwqs.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2illpqcbq.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2flncrkjo.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2fdojivqn.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2jtgtgdrl.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2rwmhzeza.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2gwymcpak.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2xznrcnwo.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2rqnmkwqa.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2mpgppzoi.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2klwgfznb.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2ucgjiyss.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2hwtfgtpw.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rvfndhmu.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2nervmwxg.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2wlvjnpjd.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2igxrwlik.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2fkdsfetn.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2vqwvyros.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2ejjsrtsx.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2iobkqbul.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2buirxxra.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2xowhksat.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2xudrmrne.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2irjulyxw.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2trexkypt.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2vcwjbulv.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2mnkjyqqp.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2zmpnohes.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2zpkzwewl.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2djjrprxl.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2smpzvnvl.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2uhymrhwy.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2iotgmzam.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2cxvgqdoa.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2vvgovwtc.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2jfijlzpa.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2nusmqsam.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2grvdzsoy.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2cqabqlfe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cifftrgv.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2misqmlsk.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2hlbcayro.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2ejxakkuw.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2pvcqehif.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2pkzytgbu.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2wyquzpkv.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2envpwpox.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2bpwqsxxx.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2tclaywbh.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2kiypxorw.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2msrliuls.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2hgcmtivo.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2skginjrw.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2ilamthwf.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2osumrtcw.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2lymhvczk.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2szdcewdv.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2egfbojmf.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2vhfkrosb.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2itvgmovc.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2ntzohkza.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2sbbgyenb.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2doohdcml.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2iyrhldsa.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2ozepampf.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2lncbozda.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2mufdzbzu.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2ongomekv.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2yqkwgngf.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2gkjfoffe.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2izbhouac.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2tsnlmwep.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2awtzjfyn.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2zezsfods.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2atvndghl.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2uethppky.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2ksoiiegs.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2cdgtnxiv.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2coctiqsz.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2qoarqaep.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2nkhxsiou.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2svufznyi.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ooychfxa.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2xgdzzuwh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2nicyksog.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2ksxjkeyd.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2dejgweyo.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2dkktxlxw.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2rqvxmwcx.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2obmozfop.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2sqofjumz.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2sahyctxd.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2wnkvwcik.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2wkfleomr.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2ucshxnwm.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2egqpkinf.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2famjyigg.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2rznhzaqv.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2ottazkid.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2jzluufwd.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2ykjmgfvm.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2mzoldfyn.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2necypgfe.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2tpogntce.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2lhfqlybe.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2pdyrwnon.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2bnidcnlm.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2djvcclah.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kmeuymgo.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2hgrayapp.html


<!-- 参考信息 -->