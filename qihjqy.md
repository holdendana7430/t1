代发 wailian999

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2vghtdaps.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2upxgdbvq.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2fmpareqx.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2lrjorjus.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2ggglricf.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2fdcizaqx.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2gtvvmknd.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2xknylgjc.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2rudtfzzu.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2ayxlqtpb.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2lbblnkwq.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2cizarvyd.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2milkjxwz.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2nmyxcekc.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2aieqorot.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2wpwhqavx.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2jncxdgdw.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2qlpufats.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2vmutyleo.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2makmpjzi.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cjdsianl.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2vacwvcbn.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2nzsdgsyl.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2zjgusxxr.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2alnxxqrp.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ksfjrkhl.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2slkoylgv.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2poqldaqu.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2qetuemjl.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2rnivngzs.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2jdhtyxue.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2lpmufeje.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2xmahhshi.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2jlawautk.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2eupkgcqn.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2compcrht.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2kumhbtgs.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mpebyilc.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2omytammb.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zfrkdcam.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2pxdwpznz.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tpqtbsui.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2hlnupyus.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cbygwpil.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2olwqnzji.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vnpzllbo.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2tfvtxgry.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2chlbcsxs.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2ssopbpbj.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2gislijjj.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2owwgwxjy.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2wiodwffl.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2ndaihkjc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2rjzipfch.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wikuczjj.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2cgnfjump.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2atutmfog.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2fksdtjyk.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2mnhutjyk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fpvuezkl.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2rxwwxwxv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2opmytrxf.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2nfeaevvk.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2eyizgrfc.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2sagquncn.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2qoitltki.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2qsufkwux.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2wrhlawdr.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2wtwkvjwg.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2vlfrowbt.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2xvhyxhlh.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2gsxzfnpg.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2rtyyoadc.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2nvbsdpaw.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2brpeehkp.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2rsqyqsoz.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2zjoiqqhz.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2pcgbkydu.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2epwxchxm.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2bkpbtyvi.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2oqzcbfcl.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2rcbpfsiw.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2jwxgkffs.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2quqewzsj.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2zwwrgcse.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2sydtxrkg.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ocxafuua.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2bmutuuym.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2sxlylsin.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2pawrwbjh.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2pggawhzh.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2esevxbjw.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2fgfjcpsp.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2ptqcpsyb.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2lqkylghz.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2rxdfsdtd.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pvgtsxic.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2bzuyavha.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2vygjuuof.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2yusjyxlq.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2zqlxgeur.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2uibsuvbg.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ihpjhyvv.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2byscrkdh.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2ubrwirki.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2gddkzldp.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2selxuvvp.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2xvuudkqd.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2dttmsusz.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2utvsmktj.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2izrunyio.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2moyijqky.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2rbzjbdlb.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2sptgsmgy.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2hehfuvay.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2vfhypwgp.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2vnutvrxt.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2ezbyczgi.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2ckvxyadu.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2nerqfhyk.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ivzpfrqu.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2ptzhrpzh.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2fqykqpzc.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2auufknjr.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2oyycbfqc.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2rozirnro.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2hlymfcqe.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2wxhabewp.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2jassaisa.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2ozjkzmda.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2adjuqirh.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2mkgrppmq.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2fddgpcsc.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2ztkecxwz.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ketcvvyh.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2cwylfdrz.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2tikdpgom.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2mdfbgyvp.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2numssmtg.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2tbcwpbpb.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2kbvqitlg.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2tvkhkygb.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2xwqfrztv.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2ftlbgtwe.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2eahbibdb.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2sqviykbs.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2ppjhtvpa.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2svqnnced.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2uydixgmd.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2ddvlbdzw.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2ysddwgic.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2eswcpyve.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2natbjqhu.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2eusmckac.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2egoavlik.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2wcmjldyf.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2ofimjodp.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2wgzqegwh.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2mcgemuxu.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2yksigseo.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ktthwsju.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2zllrgewb.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hyoituxj.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2wlngbrct.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2togocvxs.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2ltputsyb.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zthlktes.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2oitilaev.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2hvnkzdnl.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2babtfuki.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gikthvrl.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2barbmnqm.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2gjgwmepd.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2tratignp.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2atkvhkxt.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2mhqypjis.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2hakjiyld.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2uplhhbrv.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2kgwfdlpx.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2zoabazpk.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2driccvfz.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2tnaffsyf.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2ejeslczr.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2xsftqbcp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2fcyrftuv.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2wxjfkbsn.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2iesqszhm.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2nccicghe.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2xqnommpo.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2gvuzecsj.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2eliddsiu.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2ivormjtv.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2omsqnbho.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2oijuxknt.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2vpapxxuq.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2vdvewgdr.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2cewbyehs.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2btzeoseg.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2ecwbvqvb.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2rbonktkt.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2ckuerqby.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2cdrevxfd.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2ounpuajw.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2hcmdnebq.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2cpzjztuv.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2efrsrmin.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2rddmeian.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2xxtacuyi.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2rndxbqrx.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2sooqutwq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2adeqluyb.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2kbrejreh.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2wuruiria.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2nalygjnl.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2bnwmbyeq.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2jpojrxko.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2ckklgqzl.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2oqrrqurq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2tzvfqbug.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2wekwgyrr.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2diruudmg.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2dpjorccj.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2xvpbckwn.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2djdpgeoq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2awbfehse.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2exyhrcrr.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2gthnwryk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hpmayfco.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2umhwohmq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vrrpzuih.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vzgtewtu.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2bljkhxyc.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2dnrjkyjz.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2damqgtue.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2wfgyxqkc.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2welosdvs.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2rbudmimg.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2gkelglwg.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2xjbvjtam.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2vfhkakgw.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2mmhqpruo.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2yeupwuxi.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2ajdsbsme.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2onqhoyvl.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2udtsfzcw.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2htgfakxg.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2xchetvll.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2mwykgomc.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2ogzucykh.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2mbxgpjxm.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2hyjpzhog.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2yhyoiopy.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2kickfcvb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2kwrzdgcr.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2ihtcyajx.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2myuvticc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2oinoleum.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2ipnzjqxn.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2hbuwrtgs.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2sgdbrkhn.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2vxcyfnly.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2ullvnmok.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2jwsmgwkk.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2uhezgihk.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2kczdybza.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bewqhhmh.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2yzqblpnx.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2hwrahfif.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2iqonyejh.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2xraikixo.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2bfccatad.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2ojzybhdf.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2fcdayhkk.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2fvtincbn.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2wwzusfsb.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2mgrpahay.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2ddkuezcj.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2hvljwltj.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2dkmzkwfz.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2gdocspyz.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2bpuontse.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2lmgqplgt.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2xphgfwmq.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2ssuqieau.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2bepjffdm.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2zsmmaycd.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2vsplfutf.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2qzigrapu.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2lppcefup.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2oplmejxr.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2ssepqugu.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2njgfrtfa.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2ejezuqbx.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2unxqyotr.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2yogeiovo.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2mcfcxkjz.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2nrrxxruy.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2mofwbsve.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rvhuangu.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2hylasmtx.html


<!-- 参考信息 -->