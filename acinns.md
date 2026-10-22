代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2enqgaosx.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2zlsojewc.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2qqjambvt.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2sdpjnawr.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2mqyfioaw.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2cvxppgaz.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2udqibnra.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ewzfbkuy.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2wcpniyiy.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2aldtovqe.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2qwyqrtst.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2iovugmhg.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2pczlwkzh.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2fggwaaob.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2xykgcjwu.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2qcfovnlf.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2fpxbdmjz.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2hmtmsmsr.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2rpwvxsnt.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2catainsg.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2mkxosjgv.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2ohksrvcc.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2uwwantww.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2yobyieyo.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2ewoqovju.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2rnmfnbpt.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2lhehczij.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2jptbehfl.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2wvmasvdq.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2fmqldrsp.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2oyjjzigw.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2hylggvgm.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wcinqiwh.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2zqjrcnth.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2nuknrtwf.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2aphofnoi.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2htflwxrd.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2qyuumggb.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2varebnmr.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2balexhxq.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2spdfcmih.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2waphbykr.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2ruobeodh.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2xhfgsyez.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2nyoakfxn.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2xgluqicc.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2dmyedeny.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2kttogcux.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2oyutpirq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hekmiytv.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2mkmnlrju.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zobybjqx.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2oygzdxzf.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ajejzojm.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2wlhylxas.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2imvferbq.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2uevfajkd.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jgzdzovg.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2ulfyplkg.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2cuwvckgp.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2ztyvhrss.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2wadivsvz.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2iczwufab.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2wpqnpfgn.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2yhelxsoy.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2udtaraar.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2crmsahqd.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2yeuqpljj.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2ajwjbhvx.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2rsqwyrcy.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2qlsjkoni.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wykbsoxj.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2ahglwina.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yfuiqgyx.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2gooaizvh.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2szotstem.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2kkorpvhd.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2qxlklqth.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2hisrzori.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2vvmtpklg.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2ytfqqfal.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2ywxwfmlk.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2tjonhdij.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2rkcaujwp.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2fkqrhlnq.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2nmiyvvej.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2oztihtdv.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2reqwxfuz.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2fvqvpwfm.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2ukngrbsy.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2hegfltlp.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ydnsqymh.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2eiiyenpm.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2wbsxyrdu.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2urkwqkgk.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2ikpshbdx.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2qmlsjtxt.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2fjgickcx.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2wvjedryw.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2flrugdbv.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2kzxfvntv.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2ajipoglh.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2bddmtwdx.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2msobqawh.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2scghijcw.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2cpcskjow.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2iivkmfnj.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2xbldfwvd.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wbecpnei.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2haubsgfe.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2uehmmdyz.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2ycwldetv.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2wplmtape.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2dpsowohc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2qneztdhe.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2akwsqusk.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2kpgdlgij.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2jninxpcn.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2nzoqpmdn.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2einoxdfc.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2tguwpaog.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2lxordrjy.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2jdykrleb.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2guekeysl.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2afkwdffp.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2qzbcxuqo.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2rrdxxgop.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2cczfssgg.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2zkyljuvq.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2pdoydjia.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2iupbhvmr.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2xgftcjhp.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2nemkmvei.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2ryjbtaiq.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2rxkslkdq.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2ualtyvxu.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2jfaxvcpy.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ndwtmzgk.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2krlomrpl.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2vyyvhpdh.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2olfamnkz.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2ynxytaoq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2dmjubsuk.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2akuahabf.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2nwrrusxh.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2ahtulyor.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2ehjgbxps.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2dauodbnc.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2oemhittk.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2hpuvizhb.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2xlknoqal.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2skjhhkan.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2ueeqxtad.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2cunuaerr.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2smfcmnkq.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2hocnfyex.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2ffjssgpt.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2fpntsbuu.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2dqdfudds.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2bbzavcon.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2nltybiag.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2yljzxdsh.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2otgvkdkr.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2feamymqs.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2oieubrbe.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2pvlqktkm.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2lqcevsvs.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2saazwirm.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2lzstbkaw.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2pkrmahdj.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2kvfstywb.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2pztzxmec.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2oqjqxmer.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2dfdpgysd.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wbpgnlsl.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2bwodhfro.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2bwitvebr.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2aejleemu.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bpiycvdi.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2mvdoftpa.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2ivhirxig.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2chypicdd.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2twegfvnz.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2hjgqdahe.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2hadxkzou.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ygmlnhmh.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2mfdzmnuj.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2xcrmxzfr.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2pxfwtdmb.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2pdlmnowc.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2ozohddug.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2brfnhzmr.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2jkbhmazf.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2mrytjhxb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2tbcrhztp.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2opnqupll.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2lcillggo.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2zhraukod.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2okluxozb.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2xxqrtnoh.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2cvighrxt.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2eaduikdq.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2ezmpvkxv.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2njkubbet.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2dtmnyflw.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2nvlwrxfs.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2kffvcdti.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2tkegvkte.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2nrjcyeud.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2stvolnue.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2yriwrgvo.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2aagacsrl.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2lnyczbvs.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2ievtsabm.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ritbbakk.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2zmdxfilg.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2srvxssrc.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2hiskqycc.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2xodcjsmo.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2jjlkqyjo.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2wdwpzjra.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2ccrgwobc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2lbwygtde.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2pvbiqqkd.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2pwbzzrgl.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2uhocuayk.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2vdffvmtf.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2vegyfgjf.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2alcssomi.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2ekpjvczl.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ukvmmyfr.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2jdohyqmo.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2xpkftndr.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2iwmcrvmm.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2kulbklni.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2bhkojahp.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2plyyvaps.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2hdmxnkav.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2cyievwyu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jwiotejc.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2zhhatldb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bkgpokje.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mljjthsk.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2ajxhpgnu.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2pyraekyp.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2ozreyvjr.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2onajgano.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2ypopqugb.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2hniwrohz.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2gvomxpen.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2emdwibqa.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ufrojall.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kdegxifl.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2fsiqintr.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2tgrnyrmu.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2algsgewy.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2qercsprm.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2irolfcnr.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2qlsntemf.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2knzfpuxh.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2ouehqesl.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2oyibnvuq.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2xsgkzgtf.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2hzdryqlq.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2iykpvltj.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2lfmadlja.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2erquycgo.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2tltrtuac.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2sfvjrykq.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2vbbmhwkq.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2nsfaeyob.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2iftpgmyr.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2uazpofbo.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2rswcyowi.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2drmexhyx.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2lbbqolhd.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2qolgdwqu.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ivbucfyh.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2iksuwlxm.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2wgxwcnzd.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2abarnsoy.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2odghgtqw.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2pxhisifh.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2nvwhoqap.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2rnpoukmx.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2pcloqqro.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2ruxveqbd.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2dxgttlxy.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2aicavmql.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2ghgfmqvq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2ykcxudpb.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2yoiqzaph.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2cclkwsmp.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2drkaokud.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2pslcytlo.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2hwoofgyr.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2uozxtwxq.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2czzssowp.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2wxfxpjyt.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2xxyskipn.html


<!-- 参考信息 -->