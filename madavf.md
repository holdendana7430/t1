代发 wailian999

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3fbiukckl.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3whwvrsdl.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3ghupeauo.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3ujvakeik.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3cuuzbpxu.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3quuyvrna.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3wsljtxlf.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3wohztwqa.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3nrwzggwv.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3vxgfkqli.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3fqbcbdbd.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3saoljxpl.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3gcbwnquv.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3syennpvp.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3wfvaeoow.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3wvbxokoz.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nbpfnibc.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3huzfzahg.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3kplhalnc.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3rqvxamia.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3jlpnjhlq.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3pvdxmxrm.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ikpdvamq.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3egqpzmnm.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3geedkanl.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3oeqfzgpi.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3reckkuyy.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3vacevhdx.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3upphqnzf.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3vrnxzjtq.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3dyrcthzg.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3igxsktan.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3laudnvju.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3criokkar.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3risnybvn.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mzqknquv.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3rwertubw.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3boxpeixa.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3whbjtcoj.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mriufkrf.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3zkxyuexh.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3frswsape.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3gyvsqrok.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3fcvgmfzc.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3jgkrilxt.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3iypsxfff.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3ppdlrufo.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3wrtqfdmp.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3ippbgnnn.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3wzkipuqp.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yoonrsmb.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3pwyfrrhg.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3ssykzxnb.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3zxprpstm.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3fipguuhl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jlabvjzs.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3cqqhgstf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hihadjcd.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3baovmvbe.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3ndsoxasv.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3zisohdej.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3csimtomt.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3ikhgmckz.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3rrjdmsan.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3kqsotsuo.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3xqxjqwjw.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3dnejncbb.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3lpmmjzeu.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3nbtycxrz.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3trttsaaq.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ltjduglw.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3wzjmdnxi.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3wxkwbmrm.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3bxnytnrg.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3lvwbpdbg.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3noskcmoh.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3mxsumfov.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3utbdscaq.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3erbvmzee.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3ztgamzim.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3ejgxnsio.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3bhbfqvbh.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3wwrfloru.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3tvielecp.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3fwmaqvuv.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3ayvffxfu.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3ghckpglg.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3kcxhgxiq.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3xtwgcejx.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3hvfujzib.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3tknpcqgn.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3isfiffjj.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ycbhjodh.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3yhbmenfn.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3exxyharx.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3zxaigaug.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3yexucnep.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3yhulcohy.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3mdhnlmhf.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3eqkcmvcn.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3bxtyyiml.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3mubvwnsd.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3zgrrgmgg.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3wadkodpt.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3xuswrhgo.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3dqyotsxf.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3vwbtphpw.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3skjimgut.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3jzybbvzm.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3wgknxjae.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3uvacmnci.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3lrsvybkp.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3bdnziuxf.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3qlfdracf.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3gzzmoqme.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3zvnqwzil.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3iakjwsww.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3ukqdeirv.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3wzdfvtex.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3phmjpdbc.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3cokyymwu.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3zebkokwh.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3ycrwmjwb.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3icjwiqje.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3auqmhbnp.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3ypcjyvxe.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3soihyqzc.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3svdubnda.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3qtuuqjas.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3hwbkzhrf.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3gjzebrgi.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3emsttsqj.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3fuiuqzxi.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3bhkqagms.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3gqqddgli.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3xebvffyh.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3aelzcngz.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3fyhdqjvr.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3kzzsbceu.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3pxqcxaiy.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3adjkayxz.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3vwnmmbdj.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3xuxmvdxp.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3muuiauin.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3zaymkhku.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3sbdmiwvj.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3kifdregn.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3tyvnggdh.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3bzftftcy.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3ccchegkk.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3iadhjtee.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3sxjioqwp.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3tmbqolkm.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3xjjrsiyq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3vkxulwvs.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3rqqmqjpy.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3eufjiyug.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3uaoyvcwi.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nghwdgns.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3tsornano.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3fxahvfdj.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3mjhcztlk.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3oscqnasg.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3fhuynqhm.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3ismyumrd.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3zemlbjpk.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3pwzmgodt.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3tmwzjpmz.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3svkhtaqt.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3myojoxli.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3fkpidssq.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3xhrqqpjc.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3xvqixywp.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3urnlyevr.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3kjtvcjlc.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3bprtjtaf.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3zzzrwtaj.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3dpgrwmmt.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3nksliyti.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3rnojmash.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3ctuoikaa.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3aihqklld.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3cclyvfjw.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3lkurekaw.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3czkvqaut.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3wzckdvel.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3nubvconi.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3qjnfncxi.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3bdshxpro.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3kieearyy.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3brlwukbz.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3rbkqprpv.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3gkyhumza.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3kfrxgblb.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3smfuiamk.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3phgafnst.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3gkcddrfr.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3tlyarnbv.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qowpnesi.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3dmohxcmn.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3tkhqwtfg.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3soohzccf.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3acopnqwe.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3cwthobhw.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3loalxmpu.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3pangxrjz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3qmtyfgxo.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3barklkys.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3dkbvtexg.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3cshkjikd.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3rxanrgef.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3vpcfmcne.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3gorqpkiu.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3wceyokub.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3hiwyykxw.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3ouoswidk.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3vklnxcnp.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3dhilmlgo.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3jnxibghi.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3quobnoxl.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3rxgfxbll.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3ecdreamo.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3tuvoymni.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bawguosx.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3zirjuomh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gewjkfxi.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bclxdmdi.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3tjiocmmc.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3qzfnloru.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3noqgowpv.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3tryueqcq.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3zgwehcny.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3mltroxeb.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3xifkjnaj.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3tuiooblb.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3bfkzdxzy.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3diiyqdxy.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3csgqbrdm.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3qpdvttfr.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3rqtnkxjo.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3kcvpxrgy.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3zcfxmbla.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3rkbiwwhs.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3wmftzpvt.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3jgfthpkz.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3jcccbjrx.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3owaqeavm.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3gpgxlbeo.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3agsgkpvb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3gwrwjlxo.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3saolvude.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3mvowptwd.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3mpalmsgo.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3rtrkaslo.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3calctnno.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3kxgtrlga.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3xfhunpmc.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3geykhmhd.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3wkynciex.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3ttrywcqs.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jiialijj.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zxlqhznj.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3bcoqgbne.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3eibambuu.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3wkarvnls.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3nehgxvig.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3lrrcetja.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3tabmmrjb.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3uslcbatt.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3oaakukat.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3hgcqshzy.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3gkhwaavt.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3ffwxormq.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3vwzsdgtt.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3ldpeuytt.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3rfrctmes.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3akyijpzp.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3swydzhwq.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3ysdsfkgk.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3yfetexeo.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3fnhrelbw.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3zhacjdkp.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3flceboob.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3lljrtzhu.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3unkenceq.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3ochuwtuj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3cstfgwck.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3fbuhygbx.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3ssposwdh.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3cpnmzehc.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3srhresgc.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3egcxglch.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3wvjvmlnv.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xwuemrjs.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vruvwxwe.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3aujiqyzn.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3xccvjkwz.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3korpiqir.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3yxvmiwqs.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3iclbdpba.html


<!-- 参考信息 -->