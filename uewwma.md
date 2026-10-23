代发 wailian999

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3vbrryhrq.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3lfethkef.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3iekaxebx.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3riitkhaq.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3wstzswwt.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3mfjnxemf.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3oddtaopk.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3tafuyujr.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3stpaldyd.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3cbdwqfza.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3skkzcypw.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3degefhzl.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3jxptrmgc.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3cdgjjlgw.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3piazuyzb.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3fxmbumuq.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3dcxplnvp.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3wbijdfvr.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3vatkkfgb.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3swkithvq.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3nnajgnge.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3zfockewa.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3wkaaixcz.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3eafziltv.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ugyztyez.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3ibpdupvv.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3mhywypbc.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3zkmbpcle.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3pliqupzj.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3blzplgne.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3lfpbaufy.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3rrjhjbds.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3nnuconnf.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3iyfnnrpj.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3geuzwyzp.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3othfxhzx.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3pojzlaco.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3rckdwfgs.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3cogofbkc.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3dmdzwcph.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3itocaosp.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cqygahwb.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3ezjsmtqs.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ojmdxfgk.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3rxcdhqsr.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3eiwqydao.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3rljitqge.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zdvtyydb.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3ydscchxk.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xukqtsbp.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3lgyrtqag.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3oatnnwem.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3xkxdurbg.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3tnuikooo.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3coadatvk.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3rgrdeebs.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3yvyzcmdh.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3wwigpyuq.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3sjjnxvqs.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3lecopjwa.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3gkwhnlbl.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3qlxmujcv.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3cndijbvu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hzrtdlmg.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3kkynxaqb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kjdotgsn.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3iypojfkx.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3vchuubav.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3stbnljoh.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3tpquhdyn.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3wxdnstbi.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3zwvuloki.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3iyzqbvbj.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3bledopxx.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3xoryxgvy.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3iswkrlbq.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3mimgkvzh.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3iuaekuxy.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3ezegcxen.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3iogsssah.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3bptyytib.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3hthquzet.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3cvbukjzq.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3bngwtsna.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3phlmsddk.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3wfcgwdqu.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3riwrblff.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3rfxiojnr.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3foyvzbxy.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3yodrydzo.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3tkyrebml.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3wcvenhch.html

esac
来源：http://www.52xcode.cn/Article/details/gt3tzvkeets.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3uolyqpzs.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3lrzvknmd.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3lvauutme.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3ykhegehm.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3ywavuwnf.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3kgfrsotc.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3pvaehowb.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ymzthtnk.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3bjqxsiar.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3xfcgaitl.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3uowjzvpo.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3zleecejq.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3ejnijflz.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3cxtccgdt.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3fdidwjqi.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3zbcrlvsj.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3wkxdxjid.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3wbnkhosa.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3zbzwthyu.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3jpuiitta.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3ugxqqjil.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3lswkjtee.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3aidqizfw.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3twoptagf.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3eaarbgjv.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3knapvmlh.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3xlqpfsjw.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3zpohcskp.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3unrrpibg.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3ckgciiyo.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3nxcbxpyb.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3xnqipyml.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3vtbybuao.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3rvhlkhbb.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3bfwaazgh.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3nyjqibtx.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3pwvdakkw.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3dxzjkzdb.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3zhnhciku.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3ozeiqtlb.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3kzhifszy.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3wxidxvqb.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3wjvkyryi.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3vltbzxdx.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3qmqiucgj.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3fvqirhsx.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3johdzwuw.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3lmkbubzn.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3netyesnw.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3lrxtpcqk.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3jbufhalf.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3okqwvwmo.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3khozxelt.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3hwebnwpn.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3pnoyrcfy.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3qqmhednc.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3uwlohewf.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3iluhndjj.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3ssscaqmz.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3hkzykpyl.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3ralhjekc.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3ofiwxxqr.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3sjaqvikk.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3rlvarcgo.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3rscjqpxz.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3svlsdwjk.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3xcgjrprn.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3rcxmhljj.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3sgflphgi.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3dsvnegpe.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3izwpgphn.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jqkvchni.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3igdngwkh.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3snzmgvqr.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3tzvolhof.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3qgswmvmi.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3nkgkgmwc.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rcawdgno.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3luwpdgvq.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3qjwncyod.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3drlpaqqw.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3yhrygurq.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3qnilczby.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3perbrtkp.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3orrtveyl.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3glsxaamo.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3rhcihsqt.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3vsulruay.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3vstsmfej.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3ydnbumxo.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3zkgjgize.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3syzjzyjm.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3zsuedjzs.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3vamczqpa.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3hnpkrdqd.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3umxiazpe.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3abeqxiqu.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3ghlhxqss.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3aeeefbsu.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3pvowupwc.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3ewdflfjr.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3niuygbxb.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3wmihjacm.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3ttvkzgzy.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3qtmvuiyr.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3xyuqqpgm.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3xxegxuej.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3xwiulhys.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3ketjhuxy.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3netiaztm.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3onemzkkx.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3gwcmtifv.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3tbsniyhf.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tbohvrbo.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3uvfkqddv.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3yseknjwq.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3jpofnnka.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3ivperxln.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3yvspyjht.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3bqghnsrg.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3vghbwybc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3babvwlii.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3jjnnstng.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3fypsydga.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3kmiiegzx.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3zwhftsqk.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3xwhexkvx.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3knnlenbb.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3mgbwnats.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3pzdsdokg.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3wcggszqw.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3xblzdkzw.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3favlcghx.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3lfkfopov.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3zrezvbmc.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3ksgcvfom.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3dtfyafbj.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3wgadjnwy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ngzldcqs.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3skihjygv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eoreoaxt.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ahdzqxiq.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3yimqocvg.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3jvosjkto.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3lyrvskdx.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3hlkuytdj.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3jqowivyu.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3owkdmttn.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3vbzrmojv.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3yxucwaeg.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3vwllsvak.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bhtetsmo.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3toufqiwo.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3buelbuiq.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3jfzgtwgo.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3hjwkofyi.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3ncgbywri.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3tvyfgafi.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3eikmlykt.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3zkaikofa.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3dobcbeok.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3rmluzgna.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3kwpcizok.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3ghcauvwd.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3hznwaira.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3dazrxjlg.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3avqmflmc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3tsbfcayo.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3zefeidna.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3kdoxzvyj.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3hzfoovsx.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3toenjiqz.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3axnbxrxq.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3hgeqpidq.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3cglgdrsd.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dsgafjeh.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3eoisnztk.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3xmhoycto.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3rzcnequz.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3mefoewnp.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3ihaahszl.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3nccbefrr.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3zoyufplk.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3pvyxowcr.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3leitfyyb.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3duakfrif.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3jemerrqr.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3srteeqfd.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3kpccrlpt.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3smqbzeik.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3vzqmacyx.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3ncsabrnx.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3qaqwvssg.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3foobfqzw.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3qtkdudgp.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3mlvceaob.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3hqwgncbe.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3okgcenwx.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3kwlxxyyr.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ikbtocft.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3nzhumoeu.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3ejzvehjd.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3rpgbmawn.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3flegzayb.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3lqqwjubw.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3kisxbboi.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3umradktq.html


<!-- 参考信息 -->