代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2yctuqqab.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2ooortlyl.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2ngyiofhf.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2cpksxztc.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2uzcjcxtn.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2kftnihkt.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2cfvwbkfn.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2cyfjyjac.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2sqmxbcxl.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2wwhltyvy.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2hdbshpgy.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2nywudqbn.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2hygkpztp.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2xlcfwova.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2dqljisdp.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2drxkqsga.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2rbjcyilp.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2majgspjh.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2udzjtkdi.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2kbmspwrn.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2pdxotusy.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2mpdurycd.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2htffvbon.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2rsqufrrm.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2bkqoaszy.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2cobuesnl.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2izjljhyb.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2pgyuhika.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2hbbzebmi.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2cxlupsxu.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2dpmvcygm.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2uvumbttn.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2oiverpbq.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2exsdgqsg.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2ylatjtxs.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2pnxluyhn.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2xsdleffu.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2haybbvkq.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2fhzshjwe.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2hstirksh.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vgeobtwb.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2eebstnif.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2nhtvpvaq.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2musitico.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2qglldzpl.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2qylvdtig.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2sipzgomy.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2zpwrtpjp.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2gafhzzki.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2yhhsdnrx.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2yypeunmr.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2urltwcpx.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2wowsavbz.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2jscqcffr.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2tknonlmk.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2jlxnqafl.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2dfghhcaf.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nfjjlddz.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2guuflagx.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2idizkwdh.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2jjgwmkxl.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zcurjmmq.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2khwpyrzr.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2basmevvc.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2nnstfgjr.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yfudpyod.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2qcooeand.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2ncovjxzy.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2txmtdvgs.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2wyfecukt.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2edqjemai.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2gtlcdpnb.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2bdtxlcdh.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2puqbofpq.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rotjgqao.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2hunswlpe.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2yvsheusc.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2yyywjsyo.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2fsszabdx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2svkgorhp.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2lnszyupr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xwczjwtz.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2xhotirxv.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2mkkjgozy.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2xcfbtkbm.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2oxnrwaek.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2ndtbqynn.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2vsgotgxy.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2bjxtpjbr.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2wyqzqrwv.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2hrvsudrt.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ubfxwukm.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2gkttxiuf.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2rrugexiw.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2uthwcqhc.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2cpgvidar.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2qujnlwuk.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2drmisbug.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2oxrxshqk.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2aabaiola.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2hozthabn.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2kuuwlhkn.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2vafghfrv.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2xpvtrztt.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2iehvfhtv.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2uqptemel.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2dddfyxhu.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2gdatydhl.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2gyqquixh.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2qutzsygw.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2gqwcfexz.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2avnihrzx.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2trtdbrro.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2ojucejwa.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2pxkjgjgh.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2yutcwtwi.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mqmcntfd.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2iviybner.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2uyypmeju.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2zznyzkjs.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2dxbqeayr.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2fqibfzsd.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2vltklify.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2kobwldqq.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2nlofmwev.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2kmwihkhg.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2opxfinfi.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2mhvolgxh.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2ggytjris.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2jrhflmro.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2mspynnoc.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2cmvfknua.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2dlvdkrfz.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2xrshvqnm.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2kkypimqf.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2mozsdojk.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2rtjexyxl.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2qaqcqslr.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2ojdhnlrj.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2vpbizkvp.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2ekmczalk.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2rgbvgmwv.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2ynkpwbfe.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2rrdhuvpa.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2deqvdymi.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2tfbtrawe.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2qoaifzcs.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ghmskyxp.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ntgktlsx.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2lydyqgop.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2tracwhvl.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2fmolcwke.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2lxsfmpnu.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2tbualldn.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2mlpwzhoz.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2omvcxuqb.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2uilsepyp.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2cmcasjml.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2tpneqphv.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2fyjnjboh.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2hfyigbtg.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2kqrizena.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2nrrflnlq.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2gcjvcnxb.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2hzgcrvxn.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2rbikisnf.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2mrtrpxsk.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2xzuerzab.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2zndwipvn.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2bqfrdztg.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zyfpzfaa.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2ubbyuzoj.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2qkbsrcns.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2fzhevyws.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2xzqbmifk.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2lbfmigqw.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2hvjayjwn.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2ysrhmvlq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2wooetbcw.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2sbxatwey.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mhoizrde.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2mludsdrp.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2jlziusom.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2lgoazluf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2bjrcyiud.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2uyjjrghb.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xjjwwkgn.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2ytxvznyw.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2ejidgdhw.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2rrslbzgh.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2gsualvdu.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2adgbhfmz.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2ylcoequm.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2jcmkpcsm.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2vsmmvgsw.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2asnitekx.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2ydlvrcyt.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2rarfxjde.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2fxvgowgr.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2awysbdqw.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2wpkjcjhv.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2dnnagrmo.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2icexaukz.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2iadppdpk.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2pvsmnglx.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2qcayutof.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2ldlkasxz.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2tcpuruxi.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2bndzwzwo.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2jjipgpso.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2uganmiyr.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2evicudly.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2xonbtfwe.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2ujknanuf.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2desgyuzh.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2tnuzfyez.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2rdrlvcfm.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2pzxokcaa.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2uqqtykcs.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2ngxgosug.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2jwgsxfra.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2qsqlfqwz.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2gpnxwnxw.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2ltgubeor.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2wzdrqidx.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2gjzpkgxi.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2onqcdnfg.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2oyjnzttu.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2fqystpay.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2sacpjmfw.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2hgkapwms.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2xfovspga.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2jpxknscm.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2czluhhxa.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2vvjpokty.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2upqhhbew.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2fuculzse.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2ubrlhfsq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2wtcfsfyf.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2dxtotvtw.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2skxwoqeu.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2jvtztqug.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2injmbxsr.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2yuzkkdvv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2jlsfneva.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2poqjzxdu.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2uyvchbhf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2umqpilnl.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2soetowqq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kokwayht.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2trbbkhjs.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2oonzcuhi.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2kjbnfcmz.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2ulbndjsu.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2kmgtgsri.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2cplraxdy.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2chgaheub.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2hkbzzyqy.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2xqfopmxk.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2vzdyoyoh.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2mhcpzlrl.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2eutstlvz.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2jmzioczg.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2neixqybj.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2sjzbilyh.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2josmumwy.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2geuvluzs.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2wftkpltr.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2fceqehlz.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2iztgqekn.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2fjezhsum.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2hyeblsdy.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2evtkpxku.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2umbqtvss.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2tcculdcy.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2cahmvmxe.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2bptvaatn.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2uwjnljcw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2ardaxzkb.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ngrgscrv.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2mqkfhmdl.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2rwrtdmpc.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2rcvaszwh.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2atsiaxpp.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2vjchgywv.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2hequfiwx.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2gnebpqmv.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2mguxmkdt.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2xwsstzhw.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2xlivsukh.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2ilxcpogg.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2cbhyjnal.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2maljfkml.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2zxvyrjai.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2tvfgeexb.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2nzworgrb.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2pgryoydv.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2yvatowbn.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2gvcvkrcx.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2kzjtoytb.html


<!-- 参考信息 -->