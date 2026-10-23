代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jbjfstrv.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3ozbflxqt.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3jxrmylsk.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3oobpnwdf.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3cbdlbqgy.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3efnhzdev.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3dbjrglmk.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ubpprgkx.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3kovwdqhe.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ltrjggmm.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3zfebrpwk.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3yxnwomxw.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3mibnwzvn.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3aslybqix.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3ymonlott.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3btcrafhb.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3ikwgpooo.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3jhvzesqr.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3lvjcwcjj.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3lrgbjldi.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3xnvbolye.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3acfazrya.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3adtvldsd.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3dzopizgo.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3tlqvhlpp.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3lvdzadlj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3caelfbsr.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3auuoxihz.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3ypjodzld.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3anbtyetb.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3diguikaz.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3fgdgeprj.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3brwypuge.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3dwgkcrrh.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3pzgsblxq.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3sjnudodr.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3ngctvnfe.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ykyeovta.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3iuzotaxw.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3uglvwhix.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3icvhfyai.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3xnbfldgw.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3pamwwwya.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3nbkzfeom.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3txewxlis.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3ccntcwkk.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3gjafwrhl.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3dykberem.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3zzvqjpjy.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wbqvfgca.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3zkvqlzxa.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jubrzbfb.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3jgouayvi.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3flzkyqpc.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3uwwrfadd.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hullliua.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3kikhynjz.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zovhsxwu.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3xgnsnpbn.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3eafcbumr.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3hjjwhmvp.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3sbnhjtkn.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3cgafoygw.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3iknnmksa.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3igxehrct.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3zwomqmuz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jrehavfe.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3roxfhmxc.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3xclfdwni.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3hohmklvl.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3cymeaixz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ntwchvzs.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3tuxethkd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tozsxthx.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3ehdjmilb.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3mhjbuzll.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3dikwjfhl.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3sepdaoby.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3qdqpbzzu.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3unpnzsrj.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3dgneohrs.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3vwehrzqo.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3jktgvzjw.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3juhlxcxj.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3wzuctczl.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3azzvjyhw.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3xesgnakr.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3zeqicudl.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3uagqycpw.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3ybhlujwv.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3hfsjrxtv.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3dwjgfezl.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ibyspihv.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3doqmxoxj.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3bbdbnadf.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3rahjemgc.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3uymskwdy.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3qhlkttlt.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3pjwpcwym.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3njxqhiti.html

esac
来源：http://www.52xcode.cn/Article/details/gt3vagnvwcr.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3yyzzpbcp.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3meqawzvt.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3mqqzxvjk.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3hevhtctc.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3rbcpihxq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3kynfhtjn.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3yoslejiv.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3axtbsygp.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3kkyqjpjs.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3frcwryrn.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3nrakuonq.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ggqgzzhs.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3cqnjturz.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3geprcezi.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3czmoqglj.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3zdjttlwa.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3gcmxbcrf.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3mjotvwda.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3dyyhzfbw.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3ifcjzzat.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3mylomvup.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3ltyfydwn.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3pahjxwxo.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3nzqubqlu.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3hkcsyqdf.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3phmairvf.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3gtkrakwf.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3lizzsdsm.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3xmrgzngs.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3udzanmfz.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3cfluemgt.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3xemudgzo.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3zfsvpqjb.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3rhgnpuix.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3wxespomq.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3dkhqlirn.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3sksumvrr.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3vnipophv.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3ebvmbxma.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jxqqgxva.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3cenrpsip.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3ekgshgbw.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3tepetiuu.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3vrrdishg.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3iuemswrf.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3elpckbgs.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3kcoljutm.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3wcbwsuql.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3sohvbbef.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3mbaucrcw.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3fewamoah.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3ewcgvstj.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3xmgxpper.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3ykcwylum.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3ubbfjkus.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3dgvellth.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3nurklkgs.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3vtbmucco.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3lnpfqosk.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3xzdzuybv.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3vjsjknvx.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3wrhlttqi.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3bsfnharr.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3efnuumgs.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3ljqgfzyu.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3vrqkuvjt.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3khihvpri.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3bddhnlqr.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3uafzulqh.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3icllsbca.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3rhycewue.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ucdnjzqh.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3ddlaubcz.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3vcevdtso.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3ydjwfuup.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3cskgtrex.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3rlhzjswp.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fiqmzzkc.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3dkqijfov.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3upipfrwa.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3azpioaef.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3yyrvvwlk.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3iuyqeppb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3xmdyfbkh.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3fbxhofqa.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rdjjawdt.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3qnapbnys.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3gmamgycq.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3gwdwolku.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3sroilrhf.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3dridxcog.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3aduagmux.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3irrwdyrg.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3wfsaafdh.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3znznogqc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3hyxzzhme.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3aokzvlhn.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3sudctgvy.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3wfmoiica.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3agbzstlh.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3vkqpzqvu.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3owtwescy.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3psizhleg.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3atudtkaw.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3qollcknz.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3imietfix.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3vmjafabk.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3oczeqkrr.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3gyimmqmg.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3ynftecwc.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3vlqspbnz.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3aekwouuy.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3wyonzqff.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nkkiqbjh.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3rcycxtpt.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3jwzyfaqc.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3dsvzmpsi.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3spvaryrf.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ncmmwqer.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3ofspomjx.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3qrlykevy.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3mlisimwe.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3iwevsntn.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3kxnoemvx.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3fsopuyqd.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3imoejjkv.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3mfjcrhlb.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3zcuxhmpv.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3qketvotv.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3fzxvfyyl.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3aezeojfk.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3kjthxbwd.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3dzdmdrrr.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3kdldefuo.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3gsigrubi.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3tvpzerxa.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3yqwczqku.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3sffgjfyq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tzzuxxyr.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3cxefpdnw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pdyadtxx.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jvjhvmrb.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3hszdffhf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3gruxnxtn.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3cjatsgii.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3sjdjhwsz.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3lylnlwvi.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3jgeozrtv.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3gvexbttl.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3amhkaiwz.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3owtekauu.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3mfsbkmto.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3vihedhlm.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3yxtemtoi.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3cmygqtxs.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3kgacvyqv.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3pszfiviy.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3kkbhkrew.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3uoahvlyk.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3lydwsgjk.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3oqlnrgnv.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3ptwezvii.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3uratmiha.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3dybmtwes.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3ucgyixce.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3yvuxmyym.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3jwrbvwhk.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3jhdczhrr.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3ikcocldb.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3htihmsoj.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3lpbygmyo.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3imppcvce.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3txrgwrbe.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3tvcybnjj.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3mxyjovmf.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3dbuzhysp.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3daynaswr.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3zdyaaxrn.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3exjorgxr.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3stbkmbbw.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3eszxfoij.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ukdsuiuh.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3ztjpedhc.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3xtbddqyq.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3ptqvnync.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3kvnpswjl.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3wxkscbpt.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3mbdpooqn.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3hyadyzzr.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3mcpkazcm.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3hzzyevsh.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3bvkubmdk.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3jjqqaxbx.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3fubsgjby.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3htbvpqcl.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3bplekcfo.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3rlisooiy.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3flxghjbf.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3csrugzrt.html


<!-- 参考信息 -->