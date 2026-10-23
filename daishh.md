代发 wailian999

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3dlkxmhxr.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3prkxqwjo.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3zviwsotr.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3jvjgmhri.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3koyfthlw.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3nckckkle.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3xgpitkrv.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3kpvlzfwi.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3okmulwcx.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3labfyzcp.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3lkywukvs.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3qptnzrdm.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ipycuzus.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3gqjqeifl.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3xgtrjqln.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3mchhaqvj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3jwvbwltq.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3tabgjzbl.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3kqqkqpzi.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3yndnckty.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3lzdjfnfv.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3mtyocoyb.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3tjlycgns.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3ugzgfcom.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3bgbahvcg.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3izdmzzok.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3zlaiyhch.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3wdwyufhk.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3fdymftog.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kgbgmqgp.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3rkvhvcct.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cfekjzwq.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3vpglzhgi.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jixrvyxr.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3gwntcuss.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gvoswulh.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3epogqotv.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xrfzpefd.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3bzcbhhpz.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3lecnvxga.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3ryaffbrn.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3axppzoyn.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3nzxhftre.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3dpnvnqdz.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3uxqhpnqh.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3xsbddtvg.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kxcipfwy.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3uwoftsbh.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3axqscqas.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3arxdmfew.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3zgjowgah.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hsnumtgh.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3qfnlhqvn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wteosbcj.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3sttsoyqk.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3xpnvstti.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3ortpnmvh.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3ftgxgdmt.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3gxubkkdr.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3tbojvsrf.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3tcxmmnom.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3ttychwrd.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3lygwttvi.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3pabddite.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3abowernk.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3svhaugkq.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3qhtnuwxc.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3ujdxhvcx.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3dzuizwdy.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3vlcsgfub.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3bncrhgga.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3aequubpo.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3pccizcki.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3umawpfhn.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3izqpvylo.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3htawbboa.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3kbfxzluh.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3vdwdtknw.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3gjcsrlkd.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3nohjgnon.html

esac
来源：http://www.52xcode.cn/Article/details/gt3jnhhdies.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3ondjrwaa.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3rzoseewz.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3glxmwqbu.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3dfnxliyo.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3tjidvvsk.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3qnpwbwjo.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3viynqzgf.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ltaluhtq.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3ofrfztel.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3ovytynkv.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3tzzyhchi.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3eovygoof.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3stzoqilu.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3pqinaean.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3urtxjhxl.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3lonxzcpy.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3bciuwoes.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3gvbugazw.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3myqvhaxz.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3phrqrugl.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3aismysfp.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3sbnziqbi.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3imgdclcm.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3gekjjvqe.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3nhnscfzm.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3ddhohfeq.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3igcrnhgt.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3vqcamxij.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3vtcemzbp.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3alhxdczw.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3komhootx.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3nllcspoo.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3zmqrrkzc.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3nxgquqhh.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3qvlgupdc.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3ososhgyi.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3prjfpvoa.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3zqpbysew.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3dwrlmeaw.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ezcjimmd.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3uyliekfi.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3yoapoedr.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3wmvstint.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3tundgdsd.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3ypmqwnqt.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3aucqbruj.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3csvwqjoq.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3qwkjobdz.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3pamtzzgr.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3cuzwowue.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3jejfmjfg.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3skddlbhp.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3txfeqebl.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3mmdqeopt.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3qftpppmv.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3dbkvfwwf.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3rwjxgwis.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3ujggpcwm.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3kidewatb.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3uczzgpkj.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3rrcmodpc.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3atuenbxa.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3uwamucok.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3ifjbbqtv.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3qkwmpiiy.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3iocwqrwm.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3zbmdycgc.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3cofzqepa.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3hxuckbrj.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3abmcwlly.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3duxuogzf.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3uhatonbf.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3iqdwhgou.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3eyuanrmt.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3zfubcmju.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3nnnqpxns.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3wybbzfec.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qfrwtacj.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3oicdvkuc.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3zqztrkhu.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3mbgeivhv.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3nsxxvmgg.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3hhvwlfmd.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3wxehqplo.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3tkszgjko.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3zpffuvol.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3lezpsgos.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3hxkwyaof.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3guldvhan.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3bqmtvywt.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3faznryjx.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3vuvttcly.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3okuuralr.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3fbimdxoj.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3codnlwje.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3qwpmhptg.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3apfahtgg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3drzwunxm.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3hgautiga.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3jfyvcbht.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3lxuvjpve.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3sopjnhgo.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3uybqxlze.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3puwnuazt.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3frwcqphu.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3zikxbfee.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3mtoupwho.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3njnfudqg.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3axbfbcdc.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3wrsudtca.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3zuujogab.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3cxpmzhgm.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3zxwpkpmr.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3eqgrocfr.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3smkousrv.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3plbqcaqq.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3pjkcomrf.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3hbojlmre.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3xmpdgbny.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3dacindcq.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3uhpdrgsb.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3rwffcshh.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3qvycajbp.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3hvcxequk.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3ohhjfecd.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3ccylxade.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3yprvjqhv.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3mekdkmnn.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3ffudjwnq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3nuslgzlj.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3ooyfobyx.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3wivgceap.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3vsnnoevm.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3hrxmvcoy.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3vyupnyem.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3iaikbdxc.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3kaejoxis.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3bmhqotzk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qndxwbnd.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3skpefyfo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wqawisxb.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ywgiwskc.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3bwhvhgxp.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3xcrierdu.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3woiikfbr.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3uynhkppq.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3woxgszsi.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3qubpctwy.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3guotgvki.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3fqaetcbs.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3vsdtlpou.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3igkqwjnw.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3xtlavzme.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3ypotcxhx.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3viedfvln.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3uhrirsqh.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3weqrxlab.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3kqndqgrm.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3dsmyofmk.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3knzuldnh.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3qrffqxns.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3fglhjvfa.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3bseonnwi.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3nmwsysny.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3oxkzjbyo.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3cshwucym.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3fbbgppyg.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3rclvdwqh.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3eotgevva.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3vqfawfxv.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3mabrwiym.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3aextjsdj.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3hrwwwmvr.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3bfjdahxb.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3xziavvjo.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3wwyxutxb.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3vwnxvpps.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3heonnmna.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3zqcotkar.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3ohutymhi.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3oypeafke.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3amzfjfye.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3gysvpwfj.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3klqtkjer.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3pfiespuz.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3mhvihzca.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3lvzoudcf.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3kkrsjhwm.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3junsrhpx.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3kvyoeroy.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3qodysbvf.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3yycygelx.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3vyvhngzg.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3kwbwlbgs.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3sjifdysf.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3jnazqmuy.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3bcguzmwo.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3nfxrswks.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3acszeffa.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ofppooyz.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3vgtpfynp.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3jyzxzvem.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3rxfhtdlg.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3dvbvpjnn.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3tbwnmzsl.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3ctvnhieq.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wtwkqmve.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3iwfonxlm.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3cdgxiwwp.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3sltrlxou.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3doslwwro.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3ovvyfxgn.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3drmgbchl.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3vxwaleai.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3ybudqyoh.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3hvgfhhsb.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3rqrtigau.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3ostrecen.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wmfhhmwj.html


<!-- 参考信息 -->