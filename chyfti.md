代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2svadfmur.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2hjvevcsd.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2erwyuczf.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2gomauwsr.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2bjjxeaoy.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2qzqwbilx.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2vvfyqflh.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2razduhgk.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2spwlcsbn.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2tjtughtx.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2joucbtaf.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2bjwynngq.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hqdfazjr.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2hgifhtoi.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2iptrpkcg.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2dwfpwjjx.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2svghepwu.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ccgnrrjm.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2nvhqrjok.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2kaymewvw.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2oevgjaro.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2jsaweuoa.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2qpblsxcy.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2wzokbbwi.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2uodymzkk.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2oadxbciw.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2yqooipnk.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2bmjfyxcv.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2wzithdsr.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2hwhgzrkz.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2ppeueypb.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2xamikyon.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2tuyurgpe.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2hsunmych.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2cxxowalp.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2oteazhsy.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2lanavuok.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2kehdxnxb.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2gaewnupw.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2sdbkhiqo.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bvotzaop.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2zunxmnhr.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2ykhczfgg.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2dgebleol.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2ksrjujuj.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2xpolgfys.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qphuyxqh.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2rjvedohu.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2sppenvua.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2jhaybbjs.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2bhdrtvby.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2eynlhbyx.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2bccywdcn.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2icadvvro.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2nemjcqkr.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2wggvdpna.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2ooklqcjd.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2asswpfkh.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2xawdrbya.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2irxijvre.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2gjepvugr.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uvsiipxw.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2leqlxbdm.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2sdjthldj.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2rlnsihpm.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2spopffkb.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2ukkzxrub.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2tjhpoudv.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2sehsequu.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2ulxdntby.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2tthhkdgp.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2xpxflmik.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2vlrtjtis.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2ptnvtroe.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gkfxossp.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2flpbxwmz.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2lqonzkru.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2zmbhyrln.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2asuowxzc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xnazvcgb.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2tfrkqymn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vxbnnvzb.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2rmglided.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2rbcgouxg.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2artcyzpt.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2difyrgmr.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2ssjapwrx.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2iuqqrmhi.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2mdxrgsfl.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2epqwlqzj.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2xznlbgwb.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2rzryonnn.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2vzsnbxrg.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2cjpxcwus.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2kmxlrljj.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2ehpvtxsk.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2sqpgscgo.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2dkdseqwu.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2fpxslqjv.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2qgehmliw.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2yyfwcvtm.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2bpmwiwmu.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2qdrnjuqr.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2gepcdoqu.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2wpdifnxo.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2nntyyiom.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2vrmzvxsc.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ianxwsyk.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2kbmehzxs.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2qdxgrasw.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2yrfxgfbm.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2vxxqlcvl.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2oslwmhri.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2ckdcwrjw.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2nmqztdqr.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2xpxvfdrl.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dsugqjuw.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2jntnxega.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2ipryaosz.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2zfymzuso.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2jgdijxno.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2rowtplzt.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2slpqfjsl.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2dkzbcrfb.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2tcnnfaqn.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2jdfsdddo.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2lvurxvhl.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2wqttjypf.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2euzvynlk.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2sbffwsrx.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2qeusxhoq.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2efabzmlz.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2iajblffq.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2jrtdypux.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2pkjlhdua.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2ijdpjlca.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2qaxfrcdv.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2xxgfgjbu.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2rmdnxhzw.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2jgutyeea.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2skrxfseb.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2jpqqwaqf.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2smnxlhgm.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2mwvclcyh.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2ggbeaymo.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2xxiidfnm.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2lkvzvgzh.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2bceuyemp.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sivdvtji.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2terbwqfy.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2dwxqvljg.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2lhvmabey.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2skmlgadn.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2opipgpkc.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2sufywqsu.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2khfrgcyv.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2utnntwef.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2oronitkz.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2ewxmeavp.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2htfdamml.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2sshyakxm.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2ntuxpxma.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2glrkrjbh.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2gxjnaheg.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2zeuylova.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2zgzekedp.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2wffbloip.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2ijuachbx.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2cnbsvsid.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2yfmyoljv.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2chiogubc.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2gwfzbdkb.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2xjdqzkjp.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2ehdhyrks.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2ecegtmdg.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2bpxntdoq.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2oucjoiyj.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2tobibkpp.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2tungvzhk.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2cvmiezln.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2jmxjujqs.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2rfucyolj.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2wyjpuewn.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2iljsunew.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2fsrklefu.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2zjxdhxdc.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2kxnuzfvc.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2jbpdzdqr.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2rgsqbcgr.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2vypovbun.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2yytkkavw.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2envvilal.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2qqjmlfwq.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2cwjtrxat.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2yzqmokmc.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2bdrdpoka.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2kdpcpofa.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2jqfvtjbd.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2eclidpxh.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2bmerbmnd.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2cbcxxvci.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2uhiwnszb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2rfszfmft.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2pqjsrcot.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2xbaunqot.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2botzygmu.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2keumvkbf.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2sizddufi.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2fhvanltm.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2fhxyzdse.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2evxlxagv.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2qgcituym.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2tqguldfu.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2xdzlnuwx.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2pzqemfzm.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2einjtlgs.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2tjzojnau.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2podjswdb.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2wehqzfir.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2jeyipqno.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2heptdlaz.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2jorngskm.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2aworapbd.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2movkjhoo.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2aybjerer.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2vnhjyvst.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2juzlhess.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2izmakotm.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2iiuechvq.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2yxnzyapl.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2totjlsic.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2swhcjcpi.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2ecazogcf.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2vtijfxng.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2sikeblyi.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2xhsgcifz.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2wpzsqvwx.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2uxwzmfor.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2zwuzxcco.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2iqzzxpzz.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2tlsoxxqd.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2dqosgemv.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2ejpgfyow.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2nisyykxc.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2wvcxzdkx.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2davketvl.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2lsmhukfx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tavaskdh.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2nfhtdwym.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ahyztiat.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2npkproeh.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2lecofpdt.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2yhiinyyz.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2jtbtlyws.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2skcjexdf.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2tfjaiaim.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2ikxpyyds.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2mtnfxtri.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2opldrizu.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2iazohpni.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2czcrtgbn.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2gyinbepd.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2cwzpvxjb.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2hajgywcp.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2xasybnqw.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2sojzeczy.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2jccqihpl.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2wukhoxpg.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2rnklkdbg.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2ykccxusv.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2tgzmfmnk.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2umzocwzr.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2tmcapwha.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2myzcswxs.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2fldgoefu.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2jxcjuegu.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2hptexcdk.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2xohincqp.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2wsejbwgz.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2uduqbthh.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2vclqpvyb.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2kchwkndq.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2nevhulqg.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2dyvjrpzg.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ynzgovku.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2homalmwg.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2ejgfzgzl.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2ploenpuu.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2zjqdznyf.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2qtiicdco.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2keaahymi.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2cuvtquko.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ahbzdbqa.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2latymuti.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2vmdxlnrv.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2wvybghih.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2vikwfczd.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2oxceufcy.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2tktxggcl.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2nigadekp.html


<!-- 参考信息 -->