代发 wailian999

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2vcimzfhn.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2cvqpiqyd.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2vjaqwuuy.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2kmmmkduq.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2tbylmwqp.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2ojmyqiif.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2xuojqzol.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2egpvjgjk.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2wviirzzl.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2ebxsjxak.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2xrastaem.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2haxgkcbo.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2galziudy.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2hqzmqgjy.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2nnzvijsv.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2gorptmnt.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2ujqyjlny.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2osohhudn.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2hsqrjtwy.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2uxvahgod.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2ymgdwifk.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2gnbypduj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2mxcraixq.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2xbdgaohm.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2oelycjmf.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2xbwgolor.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2cycjekjq.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2mfqizrbr.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2alzqnrwn.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2oggssypv.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2nyubfxrg.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2gkwluefa.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2krravklz.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2yimbhvra.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2edmqoxnn.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2cskpflww.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2bowtisrw.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2ncaywmct.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2mjpdbzoa.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2kaglcgtj.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2weinajck.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nbjsxgtn.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2twzuyynt.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2flpooytv.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2bqgiasew.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ovvtldoc.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2zpuvlxoe.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kbtgsbje.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2pnkmzkuv.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2teolqorn.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2dfcqbdqu.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2ibhpxflh.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2mepdfxmb.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2jqjzflze.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2ljfiftwo.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2ssgtqymm.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2wzabwpjy.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2afwtvece.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jxhjzkdc.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2fvnoxrft.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2jimwrghs.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2sfvjqqsv.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2xabltufk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wfewyrrh.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2tzovqygo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2unvdbdwh.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2tlixymtz.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2cgdhkllw.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2qrcntjsv.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2gjatjbbb.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2twyyigjy.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2wavckjuu.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2xztnqfkf.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2jgdikbzk.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2uorawkoc.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2ndosihas.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2xzxaiqqq.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2vfsuwvyl.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2nsxdeedv.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2vuhsvurf.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2symnjlax.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2xgnknimc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2qesjpygv.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2wizroyrf.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2sesadvmg.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2wsplseza.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2bkionllj.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2jvxqkhav.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2jpxrgtbr.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ffjfsrbk.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ebunhuop.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2wpriknzw.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2knsbwgco.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2ounnovfk.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2fsfzuusb.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2abdipdgb.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2aclkxvdu.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2ouymbqzm.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2zjhnaxfv.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2sewwmfic.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mldgkukp.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2gvztxqhl.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2tmdynori.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2gneurjqy.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2bpiitlsi.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2gfmipsof.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2wfkbtvtq.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2zrppckyl.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2yyrefaae.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2onbxjstw.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2vomdivez.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2gybuiuox.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2ruqqqznm.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2rdktvuux.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2qnzzbjkz.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2hjqomdph.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2gmnromoh.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2kgskkexw.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2pzlcekza.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2jnvkkzgm.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2eaimufei.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2bvgqfmnl.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2ldinyisl.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2krshiusx.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2isoglxcu.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2fxslsiyu.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2lvwarwei.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2mduvpizy.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2dwpirdtg.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2arapbngo.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2ovcubekn.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2udljeajn.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2yqmixptj.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2vsdurlao.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2xxgdyuas.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2qnrdwqvz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2ljtkiwfx.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2ciebktgu.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2sbfqgzjm.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2qoublqjb.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2yiydaixx.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2lveazyzh.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2fqyzfpeu.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2cqxihdsj.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2aijazqcy.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2keougvud.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2xjyxzxak.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2elrdyrmg.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2bsrguyqz.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2qbaqgrjn.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2gmlagknb.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2ucphhjjr.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2gcybwnrr.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2actjjagr.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2scuvypjh.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2mfqwidrk.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ssxtimgq.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2cwqqoucd.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2fppaohue.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2imcdzrbf.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2bmrresej.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2qjbfmtxw.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2ewglrcfa.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2yjfzikht.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2diolxkus.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2cxcgoxdu.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2lpzlkdrh.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2vrfodhen.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2npmzcbbu.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2fgyafqlj.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ouhgjanc.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2lzmuaujo.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2idjkkqca.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2bwhajhnt.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2nipktiti.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2mmsxjutc.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2usugbzqk.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2kmjvheyx.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2eypkocgn.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2simhzpjf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2rfsmlqyo.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2olzozlep.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2xwykuxcv.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2rhjflimm.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2jqyinxdr.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2bfyssrer.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2iurrnrrl.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2exrkmgcz.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2nighwjhk.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2kfyxpakg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2simwyuts.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2qgoxgfos.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2ylsazntx.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2iaihndbm.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2dzwkqkff.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2twokxuyo.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2thqwxkms.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2xakywnbe.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2wvtrlgyc.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2porshkar.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2mlyoywcm.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2dfyfuwzc.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2flcuhnuf.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2bdeyjxgp.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2xochdbxs.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2uklnfppq.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2yallptdx.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2wnjsvkrk.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2zhjwtnwk.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2noekcgjh.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2rbzhbxbz.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2mdzhqfdu.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2ixhilwej.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2roqlpwot.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2xczrozxn.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2znvgltvv.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2bmmanjiz.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2nupgnuzv.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2expbsijl.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2xqeiwxnw.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2jpccjzyp.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2lktonjee.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2hfsxksbo.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2maixptbs.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2rscuclfp.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2dbqctoyv.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2dbtxqnpn.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2qvtjoyck.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2ymbdhdnn.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2kkwdrdqx.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2ykoxyaoo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dvpcwfys.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2pgxyjkuh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uqsonens.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2shycmyyu.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2kfcmlpwq.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2izvcxtaa.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2oiwgsuts.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2bsyndvup.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2dlrpynkf.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2znxscegv.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2oupvoihp.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2dbfpspsl.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ptesjwiz.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dokcovfq.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2wdewmoxi.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2bswbsbkn.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2qcqztxxm.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2whifewxc.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2jtvmzlcs.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2wlmjzflj.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2duztvsxw.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2sumddsdg.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2xlqhksrx.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2myixbypj.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2zrucutxt.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2mfcylsuc.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2pkzhfjxm.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2ieixpcvl.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2wvbnttqg.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2hsqtphgt.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2drvvjamg.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2talwvlxt.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2uoqvowqf.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2ozhczkuk.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2knwmemga.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2icbfdvfz.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2kyqwsfbj.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2dfucaolr.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vjkjywux.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2ckxonphv.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2ylowqzty.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2grrgmwiv.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2hkqrtqsu.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2nuxoaxud.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2lrdhqwxz.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2cdjdifih.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2ckohevzk.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2asxcdgtb.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2cajsajwz.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2aymsejmx.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2kayiqaae.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2kgvupphn.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2krghbnst.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2goruozvr.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2miwfscjf.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2ikmqlhak.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2wvydruzf.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2kyqousww.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2kzjyhktj.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2bnwldisj.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2wnlqehxq.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2rjwgwtsd.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2ozecsazn.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2dueyjknc.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2uyavtxnb.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2uuigznav.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2ivksusvn.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2vmyetlmq.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xuqssvqi.html


<!-- 参考信息 -->