代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2izaevsum.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2igpigyhx.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2hqekjvyg.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2roesbpzl.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2lqkdyhas.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2saerduzf.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2cuhedqoc.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2yqccvhae.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2hnijkbft.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2pcqjzzzr.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2abaxyfif.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2szfvpdyp.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2sicmnfvu.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2fxoynsyx.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2ryyfxcli.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2qkhznpsv.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2syoumoqr.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2pvaegwqv.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qilryytn.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2mfmndgvy.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2yxzvrvdg.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2nasjamjv.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2semmvkgv.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2vmgcrkny.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2bgfqlvsj.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2lnkyjwnf.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2edfurmmj.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2frftlkht.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2wjexigfn.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2gevmrjni.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2zcnbnktg.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2qxxcljro.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2sikizmwx.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2sdclvviu.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2bglummce.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2ytmjyboy.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2oyscqjuu.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2gwerzhzr.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2bfzusttl.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2pkvalzjz.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2glgsgcxh.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2llwwrlyr.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2dmschjrm.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2vzwmlvoc.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2hxkodzlw.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2bzrpthay.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2gekbmuoh.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2hjgkilrf.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jptmatcg.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2bybvfapi.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2yeqydwcs.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2vzzuibiy.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2rvawzuho.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2zkejecfc.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2gamzjpjk.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2kcrhgcee.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2mlqthqjo.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2dldoflci.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2hdafnjgo.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2nuknsycm.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2tulmdlsf.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2dnemwemv.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2jqnrcizy.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2nxiylalv.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2gzjopmfa.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gvjyjuat.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2duxqgnee.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ysjfdlps.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2vtdntdzr.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2smpbzwoj.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2xsqpugii.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wmbwrqrv.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2ytqkcfvv.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nfmvmeqa.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2sdjramhq.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2jisnorfu.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2tfvohnst.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2ghxcerfs.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2jrmoffjf.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2klcnskwv.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2odjwswse.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2bwiommuh.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2aeanhxcy.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2wozanxho.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2lnxkrwnx.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2lyfhqkjs.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2tdfjzpwm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xhjuijrd.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2hcehhhzm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2anbwtlem.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2hymawnhk.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2razvuzry.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2zkfkuexj.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2febaugry.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2nzthhlfr.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2znumjcii.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2qkxpevsy.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2mcgdgqnu.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2hcsggpji.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2vmshzzrz.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2qqtdhkgr.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2tyvtknry.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2fthqonep.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2iqwrvlpx.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2keveiujz.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2ezcdqdnb.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ezdtyxgb.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2krqetaoi.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2mzxfhxrj.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2eamuayuy.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2zxdowztv.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2xxohnmtk.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2eghwbjxa.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2okpxwzgf.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ciaojnxf.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2vhlnljde.html

esac
来源：http://www.52xcode.cn/Article/details/gt2egwkikqy.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2yjfjtddu.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2trucniad.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2lpchxawm.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2lrixeazm.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2srltkpie.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2lrnqefbs.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ppwvicjv.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2kzygxovb.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2szikrdoy.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2uhpukokj.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2gihwnhfr.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2adjjvtcp.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2qljcohbo.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2phuebchj.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2biylcnbe.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2hkmgqtuy.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2ywwweoos.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2aislvcqw.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2usjnxyga.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2jowiicxs.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2gcbvqhwn.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2iuyzfmze.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2cqwzlncm.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2huhweohp.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2nzwwvlic.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2kgmylgpy.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2iyvqapbk.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2hdipooyf.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2ylflhier.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2xafszbdd.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2aoqlawca.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2mzfbdeov.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2knmnnbfy.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2pemurwgl.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2jechdjwa.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2xjktnrzr.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2pcovsntz.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2ronehdja.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2patxcrsw.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2pneuyzhm.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2nbpilkgy.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2loeacrqu.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2crxjzqzq.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2aztampnd.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2ukhbetqz.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2zizymrkh.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2uvabuvlf.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2surpxklx.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2bmsbkxpd.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2hvtfvdhe.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2wosewklm.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2wuxkihie.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2jrqtxjkn.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2ihoqzvcz.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2ngxvsvsn.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2ydcsxjod.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2nvhgnvtd.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2sddaoukl.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2qhzxiqkz.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2hglaxbdr.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2kfqstgli.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zhgivzla.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2sphyvwhe.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2vtuejkew.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2wxewxrko.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2xbswaljw.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2clfagato.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2mmmqhqrs.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2hibgjspp.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2githvnjc.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2qpjgworv.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2qpohpdjt.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2lqcktmwh.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ziqflong.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2fumcbnts.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2cmanfhup.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2xjcuezom.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rlftrtgq.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2jhpznkhh.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2cbrcmlpj.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2eanmekii.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2iklnxflk.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2afijchmn.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2gwxdyqlr.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2vzpubjlg.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vcuqflnr.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2aofcgvdn.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2rpbsvaps.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2mwzlrdzi.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2ohmptdbi.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2wblgmocf.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2fvjaxqbd.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2nexaoeja.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2zaoloshy.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2zmcwqhzf.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2ggahvldv.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2hocgbgkg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2sbtjjqkt.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2spasypqr.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2woxrfaoy.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2sapyvfum.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2yszhcljm.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2vxpghdmy.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2tothyvgn.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2qiuimkhr.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2shmbjzdb.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2slcpezkv.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2eogxjkae.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2pwhqdanh.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2gfeqqtvd.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2jfprbmnx.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2eozudhcb.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2kbdrudvf.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2bbhgvcez.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2bsokvuop.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2mescalxe.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2wclewxto.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2rmvztbfu.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2cdyxgler.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2qfzjumxx.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2vjffjfoa.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2owrflgun.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2vzcvliit.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2geiliast.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2umaeiszt.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2uspfsemk.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2udplidmm.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2raplwsuw.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2qgeuptfo.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2jedmoopi.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2mhmhqdxk.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2zfqdmoij.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2mumbypst.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2cqpbbkvm.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2qewrcftr.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2wgpjbxgx.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2kzbxcikd.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2wgictchy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zsgpqxvz.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2wjxnxyym.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dxdohrck.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2duzraitp.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2dtkqjocm.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2uvziskbg.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2ktaodwkx.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2jxumhujn.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2bjiemwxw.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2zkzxkncg.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2ukgxewul.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2djajnscl.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2vzofwraa.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nvarefiq.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2gtmjgici.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2fhlefohn.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2mhhwuhef.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2zspwyvsx.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2wygpwann.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2jbfmtjhz.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2sdocighx.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2jodfdmik.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2hmndllqi.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2awxnmgqj.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2aykggbjr.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2ryzyvtdh.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2wjnhbuka.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2vgaxebvi.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2yjnoeoki.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2wxutuxkt.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2lahvoqiu.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2arggvmtt.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2luikjeqf.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2feqengjv.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2nlqqfedk.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2ldfrlapq.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2gvcknygn.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2fcfdyvmn.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2xleloikm.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2rihxlzvm.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2fizvwgoq.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2fbkixirx.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2gzhlcwex.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ulkhqled.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2nekitxpe.html


<!-- 参考信息 -->