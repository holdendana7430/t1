代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2oboijdxf.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2fqwqbznt.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2cyuxdpti.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2doykzdww.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ihdmpfaj.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2kyqiwyle.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2kgthlukl.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2hsaoeegb.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2sfylzugw.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2qoqldnqm.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2sbelubdz.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2rwrtrotl.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2hlkgoovb.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2bauqrblq.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2gcuygyad.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2nwmepfle.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nwwpluoq.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2qlzjfjbh.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wgsahphp.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2ensgaqny.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2myrupneh.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2cgsidfbs.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2gvqrytsj.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ntncnjwl.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2fazecqfm.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2kmthoyuq.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2yazucoes.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2hjnwtbnd.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2fvudrrau.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2zkvjxelc.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2kebcskyj.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2zhfanzbw.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2prqbvydy.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2vjggqpyv.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2tgxqanwe.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2jonkwugq.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2qynkyqvx.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2uisqguni.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2spnwqdxs.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2kkrhceou.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2wtrduhje.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2ofyyvist.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2pyoibqsv.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2zlmvidya.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2lykibuic.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2ujwpotsr.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2xizishvx.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2ijbieyoe.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ctlozjiy.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2avuhjzyh.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2pmlfijxr.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2zabkzeon.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2sdjvvbml.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2wksjirzl.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2fmexwolt.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2dqeakqij.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2kbmxskzf.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2orjygrpy.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2hdaonmru.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2gpsiaujk.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2pthmgvhc.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2kwvxwepd.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2fdbktvev.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2wdabwzfc.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2tfbzxzlj.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ohgpurve.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2ekufcnrn.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qdzokhcl.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2oedemgjw.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pgjuwiwu.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2zqpfirhr.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pbbrzvbz.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2fdjlhban.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bzugnhpa.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2uctgeywe.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2cioqornw.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2mpcxepry.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2rowuorvj.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2nosviqnv.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2khydlfrq.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2ehbqhsec.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2lajvskme.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mxtsglul.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2heorezzp.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2xdhpehwd.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2nteyuldy.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2voglrcoj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2giphzdba.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2yafzxhxh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eunkhkxe.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2xdtuhlwk.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2dcdfashx.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2oswhxxuf.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2ibusryia.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2evcnzrqo.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2swxmvfhx.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2xosgfedb.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2hwbbblht.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2lpbdilwt.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2orchwhxl.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2lvmnmfcx.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2goycoyhq.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2oyqehckv.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2qdcudftg.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2rlloycgd.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2ehzvnrjd.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2qugodrpf.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2nemvjdqv.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2izkwfsqx.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2vldomkca.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2oozcmmcq.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2dmzpwfci.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2ylbjiuwj.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2zwemtjbu.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2kaadrjmm.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2qrvufrth.html

esac
来源：http://www.52xcode.cn/Article/details/gt2wyxcqzlq.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2cifusmzs.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2yfrrbsmq.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2bqjretbv.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2fxalbhld.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2fycscuhn.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2vyzunabs.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2xgbfzydi.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2oveqbqvs.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2rnxcplae.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2ddebsfxr.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2ymeaugjh.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ezzztskp.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2sowjwnay.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2rkxyqwpf.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2wpgokgor.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2oewdkiwu.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2uhsugnor.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2idrgnmzc.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2mffuictm.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2pdfcfnqm.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2fnrdcgrj.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2epspjbjv.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2otgbxbdw.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2fuqaljct.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2kfjqpuhq.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2uwtnfhor.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2hphfjcpa.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2kpurdjco.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2cusntidd.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2acdvhakc.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2aekksqxc.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2lgtjofbp.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2kcxkyteu.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2busrwmwx.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2rwzvmhju.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2oibrsxqn.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2pxkxhgia.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2okmpwjqk.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2tklllruj.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2vjzzfwfe.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2rgwdiflq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2gfdbbaja.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2yegzmwxf.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2omvpuoxb.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2ycnxxsnk.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2dibkjtmq.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2qlgyiylr.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2xlpnronr.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2kdwpaixr.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2lnvosbgv.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2ekiujmrs.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2vujdtkjd.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2cojimffw.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2stpourxu.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2ucetpjby.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2jbaozyff.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2djziqwoi.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2cmjyjpwb.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2yksqhxxe.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2ceizhqbd.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2wdalavty.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2pdtdgnwp.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2hbrgdbso.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2oqerechh.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2fropzlkq.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2tphsdish.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2lsbsyaus.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2cqnhalhm.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2wfhnfvzd.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2yugxcmgi.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2wzosnspz.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2dndmjfvw.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2hgflbfzu.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2rpzhjgwo.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2igeofhig.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2shjtapkn.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2zvbdmoys.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2szshradi.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2rgnzujkb.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2ttsvcahf.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2jiijsrty.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2mfmpddtn.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2nanpttjs.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2ofvbuagh.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2oeehttrb.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2fpqteozj.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2ktytjasi.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2zlurawzl.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2gegdautl.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2xisqjbeq.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2vypkipqi.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2bmjnitrh.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2dpeiggdk.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2cjwpsvhi.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2wnvgftoc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2ybliittq.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2qvjrikyf.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2qsnjluvs.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2slobwpjd.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2yliokffq.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2bxpbkeii.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2vwvlqkdb.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2trpaigrx.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2fwrbnsux.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2mrnesanq.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2cobitfnv.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2gmdggjuc.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2wtpnpykl.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2kxmjvhtd.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2stxkzean.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2lsmtolmb.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2qunuvnfp.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2tgwestay.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qkmnrwia.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2ugsxyqlz.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2uvuhxirm.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2hqilrjis.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2wmqibglr.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2poyyqlvu.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2etvjazfb.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2yjpdfqxq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2motprvre.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2qirluoug.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2jdlmgkyu.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2xkkdnixp.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2jrjdlvjz.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2vxgxnukc.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2kwvckuso.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2xyyihcqz.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ufkzuhvv.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2thbbjuzw.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2jgbrvpqs.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2ddepfqlp.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2ovdawidh.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2ybyedyln.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2sojubstp.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2qvytwayk.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2tuucpmkl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2awfornmm.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2ojkfypjm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2owkjestv.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xrwrvzuf.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2kmcfwtgx.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2hbxcnwyd.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2cjqhqrgq.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2rmjvjmky.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2vmnwhnim.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2knhbxbwz.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2voftoshq.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2tivslmow.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2jjlbcqzp.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jvbjoyhe.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2synnfnue.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2ltrarjbz.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2cdrmwpev.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2taffikvk.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2lsuwikrj.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2qzyhxyvx.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2mkdopcfn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2gjywrspo.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2bulsgeiz.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2vznssyox.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2dvjxfrie.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2rurkftya.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2djbophvg.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2dhpuwxwd.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2kddsmtyt.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2trwsupxm.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2gljnglrb.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2euwibaxf.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2fobgcrzj.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2cdrsombj.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2cmfyvatt.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2pxvuyhfb.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2sdjxakje.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tzcpxumn.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2orkcodpo.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2bsjojwzn.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2moimgxay.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2gqfwmovz.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2cjgjdsbv.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2itqizxja.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2yujvczbz.html


<!-- 参考信息 -->