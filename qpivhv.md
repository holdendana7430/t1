代发 wailian999

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2xlrmcwqo.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2isqaecpd.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2mlbictdw.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2nqahwtlq.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2rfvnhfxz.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2mvkqkhmq.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2vvrtvlnp.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2gqlkigyy.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2xqbnzpmi.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2wxzkomau.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2lpyizlwn.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2hkklranh.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2hsylbqjj.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2yuscbchp.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2yxfpwehh.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2qgjtwqpf.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2ekkxuhra.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2zfjahzyx.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2lgwvgdaj.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2ovdwozfu.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2caqvjchp.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2sjrlypda.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2xpszqovq.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2czsnvolt.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hujykqdr.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2itynbrwb.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2jgwauqdx.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2apwbksgl.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2iyajkilx.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2tfsntsgb.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2jolgoxyj.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2gwsaidml.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2vkhirfmr.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2tbbrvovz.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2vzpvuzbd.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2xqscldxu.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2bphqpopz.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2alahrpeo.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2vaemaqcx.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2tzchmkol.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2waimkmfw.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2huadqgsz.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2mpjtmvme.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fjqreklu.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2qxfacewr.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ofuenpdv.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ppvtyagu.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qbsnftwx.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2wtgfhent.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tbrfsyzq.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2oexuqcmi.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2jibxszqw.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2rbolqmvv.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2asdvefjw.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2khcnhcim.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2whsmglmx.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2wfioqjpx.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2brwfkfla.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cxlddwth.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2bszzsguu.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2wojmgdep.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2nfptfump.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2mqlvdgxf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bouufngr.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2sembnluj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fxuzsciw.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2vdnlwpny.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2eveydeyw.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2hhskfqgu.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2yajffadj.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2igvjqjog.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2oiljykre.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2yddbsgyz.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2dekwufdr.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2qrtwdpao.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2dfsqiuhn.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2xpoxrixh.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2weicczrm.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2fcxuadsz.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2lpdrspcg.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2myqouzfh.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2cwtiyica.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2mujiczwy.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2crczntqs.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2yocbvbva.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2ehdplpkz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2agxzvbcl.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2thwuzimy.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2whygbjwk.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2naegpklw.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2mearmvpr.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2nctlfvwy.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2mhiuahfu.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2bormbclk.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2ezjilorh.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2vcuuhesy.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2crodmpxk.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2bcsestwc.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2hxfvfwft.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2wwhagzkx.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ttczkamd.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2webckrbr.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2mrlafckq.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2wnqvzyhs.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2oqdhfnph.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2zdrptqze.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2zfkcymnd.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2jctvcdvm.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2awfxyjll.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2jantciok.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2xnzzaqkt.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2jpynjlsq.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2vhgszxsp.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2vfdlhkje.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2wowmcurq.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2nfpbzoor.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2glurgxpq.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2rfbhzppn.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2uochgjks.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2vchetfuf.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2rywkvumz.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2wlxgfjjf.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2zelozcei.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2hovqjzst.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2dzjmpuoq.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2gkqmcyic.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2usdtcvjk.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2uipwhxfs.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2vtrnyhfi.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2jkynctha.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2hzunpldf.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2okmukvjs.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2jwjfvoye.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2nrfjenvs.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2kytvagno.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2mkshmtpi.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2oplrowms.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2hhdfyxpm.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2xwammfft.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2nigxfpod.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2sntslapw.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2lfpegrrd.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2ajhbbcko.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2hxgvwarv.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2wlesccaz.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2tqupvsdt.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2idizgeki.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2tskutxdu.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2qgfmprpa.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2htqyushj.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2fgbwwxoz.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2lydguqte.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2howopsgp.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2gqqehefc.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2joenarfv.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2iopnkkzd.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2ymawlbiv.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2veziibdf.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2cqpisyqa.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2ydkrynhi.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2urnddtsb.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2asjyywpc.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2artvywbz.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2ewvisshh.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mqveahtt.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2ipkethiy.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gcqyxwsl.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2byfscgyo.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2cwaycojy.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2gknhsyuw.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2mntdyytj.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2kzvnkdvp.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2tkiwigzf.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2vylkcerc.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2uimexisg.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2lwxcvwgb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2iggkdgvt.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2jzxhawew.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ltvmhvue.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2ygpnpoxg.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2fnutzndp.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2xulvmvwb.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2zaivwyxx.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2jucmxxte.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2voyhnxel.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2ukebzwos.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2qltcyclf.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2hkspitez.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2zwgtxwju.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2svgcxpie.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2wjfhniaj.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2hynplfbo.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2qjsrzgyi.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2xbkogspf.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2typjnodb.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2ourjouql.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2rbxwyiqo.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2eypewnbt.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2stgrgtdd.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2gilzovlm.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2wuhooqem.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2jcjsrqhl.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2unxwionv.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2biiumupp.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2xjkmgogn.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2stlrujgs.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2nkernoxk.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2clkslebw.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2aavglyqz.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2cgyiannt.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2aehxvqpv.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2iizxqxsf.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2pqljdxzt.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2ezrmhpeo.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2bevsjioz.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2shovghmj.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2ueiuxrjj.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2mfxaqoth.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2oeemlxwc.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2jcvxgpof.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2etfiixyu.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2ibvpaozi.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2mjxtftze.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2cqjpfuqu.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2qrvqvjng.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2wpmzceki.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2ctzmmhnq.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2xnhpzwtx.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2oekpwyvm.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2zcrxzmnu.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2wfolnmdj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cmwhsasc.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2oygijrjv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2msrngyjo.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2mrbhlszu.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2nkufqpjw.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2dhaucqvp.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2jjxaqgnq.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2fxrzfjox.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2vkdlscsh.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2ugedjlin.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2wedjlver.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2lvrsbsxg.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2jbahzhdz.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vkidqiuq.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2fziylaqk.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2rqncnmac.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2knpigewv.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2gnmlpkeq.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2ivjryeqv.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2xlkrugao.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2fryzvdfj.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2skiefupx.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2jrqrcnmp.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2jrioofbz.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2mdwmebou.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2blnmlfxk.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2igmegpyr.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2ygnegdol.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2drvssuwr.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2pwlhvalt.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2uvtpidfs.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2tymkfdio.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2ucskzggq.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2uzolbxdl.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2eeufrfok.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2vwgvsejp.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2yjsckjfx.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jmiierrn.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2anktkwil.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2uykunnrw.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2jusjgosj.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2kfzifcjo.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2yolghhgl.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2nxxrynhv.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2ekspoamy.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2xidszdsx.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2pjqssfma.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2gvciikzo.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2ohzclxax.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2vnrytrdm.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2ytewdafb.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2ybewggzz.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2jpclsnfq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2abhxqnqg.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2zghskygr.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2qlkjnsvx.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2yrfeamsf.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2cvgefmoj.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2wjuntqlo.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2comkxxxd.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2itynsngn.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2guikziin.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2ajoxvagc.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2yvbejyxk.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2dcqdxiwd.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2eszfldca.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2pakbpmro.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2fsvnhksm.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2deuuoioj.html


<!-- 参考信息 -->