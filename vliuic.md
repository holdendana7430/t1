代发 wailian999

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3vwnaowrf.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3xepwtlmh.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3wguorfan.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3vdporobf.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3ygzwsjjf.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3agcoklpd.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3rhkftgjx.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3eonfyzdf.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3dompzrmb.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3oggwlikx.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3dtxfrigg.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3kyhidcrt.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3mkjopomk.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3qnaxgiju.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3oljxihlw.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3jwhjzvok.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3kafachiq.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3kndlnmbu.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3qcxffxax.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3ujnmyktj.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zocokbgm.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3zxtcpuzt.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3rknwpbsv.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3nvpsshry.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3npmwonew.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3lesefthi.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jplfkpxd.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3pyifrdji.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3iwfxjwcn.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3mfewtcae.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3knkjhats.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3jhfunrtg.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3gucrmuwr.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3wtzpxksh.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3pkrgztbx.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3ebrepjbv.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3dcxbefbf.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3crnixdna.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3ycqxhrrw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qtbldnjj.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3cqtneglx.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hjauhack.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3nfkcjbqu.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dpfjfwiu.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3xzxyhhve.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kzvjfsai.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3tlaqxtku.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3txiffsiw.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3oqrjtldf.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3uesjhzvr.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3jiduouxm.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3kooamcgf.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3kizhmyln.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3mdfhjzfz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mvavcvwn.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3hhakrmxz.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3ponuzejb.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3sexadoqc.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3jwxmbklj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uuverdbs.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3wgrzorry.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qaadnqzk.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3bjxzqjio.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3pgtmfxzw.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3zdqxyjdu.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3itbgkvxd.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3dclnppgz.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3pqjdhdnu.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3pnjzvlxk.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3jmbztrbl.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3yracrbxx.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3jlovwqye.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3kvteggwq.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3wxdggknc.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3qclwzsql.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3irssldsj.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3rfnqzyit.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3piljhdtq.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3oljkyijh.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3gjjdcmmk.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3gwvotqmz.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3tcfnugcr.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3kioenplb.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3znpacxzk.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3htoqwbau.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3rujipznw.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3ebstidtq.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3pzveytrb.html

esac
来源：http://www.52xcode.cn/Article/details/gt3xnqeekrd.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3cxmgrpet.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3fnsinydj.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3kwnmcqim.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3yrijuexw.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3gpcggvtm.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3eimfmpsm.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3oxdrcrzd.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3clwjnnro.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3zlebfvft.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3nljzhcxk.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3bhqhwvoh.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3saemscuo.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3anvadcvh.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3belalwnl.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3bmmrksvo.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3lynqbozd.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3uirenpsx.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3jfgucnvh.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3wscoduck.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3tcvvitjv.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3vqxwqtpj.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3bxgbqiqn.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3fjbyyqjk.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3iicfgmdc.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3lzwtlpyp.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3ptnwnknb.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3unfiazzw.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3lkcogiom.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3tbesrgxe.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3okbfnwyg.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3fugiriur.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3qaokhuoe.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3dkrhyftj.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3wrhzgsdy.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3gofzppbo.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3sojcrkmk.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3ygaedqqc.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3afdvtkat.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3udnzdnbx.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3lpsvxpib.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3bgtiflii.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3gpzxrcuy.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3aacoehck.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3diaueqjs.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3menkfxpx.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3uetjvuid.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3grbdsnor.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3knrrovlf.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3iypiqcyp.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3wkgeykbk.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3qszewkfm.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3zhxbhpyu.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3utsvcptq.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3vptreydd.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3oxobpdye.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3rkccmozn.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3ynajyrxm.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3faeqbklb.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3rwapzoyw.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3rgndmwzh.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3mxsrbxjw.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ixdrqohr.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3qqobwiwi.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3bgkpnfsf.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3jeqdkedx.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3aoxcenlj.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3xuhxvbbq.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3gofynbxy.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3cpnbtzux.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3wvxphzfl.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3boknvqdw.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3gnoqpeev.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3zjcniyfh.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3cdacwtme.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3kwxxdphu.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3astanrms.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3ybgmdrwp.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3etrwprss.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3qzkzkqpj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3vwrtypuw.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3arllkbvp.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3kqcbyufr.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3wjqeqhsp.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3rugulnfj.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3ratjvzpa.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3dqalbkdk.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3gqjcfqwy.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3pjliocez.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3alwxftry.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3qgmzimhc.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3uquihfix.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3uupruwqa.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3xqymchwg.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3zzrplgyj.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3wgqduyxh.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3uqzvmhzv.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3tbzgergo.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3blxxxluy.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3ejpcbuwu.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3ecnidxwt.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3jqdenddk.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3qwsumsor.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3wnzhoznm.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3qbhmmglg.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3kxzkidtp.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3emappebo.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3kmevymih.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3gxlqsfuw.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3wygilhmw.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3wqbmkexj.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3pdboqmlb.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3fzspimwl.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3yenvecwt.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3pzceetzs.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3elyeptne.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3lelizesv.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3donhellk.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3mnakxlro.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3irohlujd.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3lslhdxdr.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3mfzekkhk.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3vsegykvn.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3cqrncgye.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3iiofgzjv.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3obgcceav.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3oczlvfno.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3rhsewyuf.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3frnszwew.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3yhwqrxnz.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3qtglbcly.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3qvkbpyuc.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3omgltxdr.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3xttzsprr.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3kkejxyyc.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3ykdrvrri.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3zgurcffs.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3cxtyxhws.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3pcojnyso.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ixqvikmn.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3qyzgfwyo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rnuggotj.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3leoamcce.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3pnlpltph.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3xaruwizf.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3ztgvtqlq.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3mvyhxcsy.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3udjukytx.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3ehsyafbd.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3lesxjxel.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3mfbzodbw.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3htowtbnj.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pmbvznev.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3molwmurb.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3pxcubelc.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3oooahdis.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3gyqdrclb.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3whrgyvsr.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3cctkocfq.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3ngdflsli.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3wjiguxzl.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3sptjvwch.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3wgxfpips.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3kfoksmzz.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3qyalznob.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3dhbyiaim.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3kgbhstjs.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3mbdvsotb.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3uxgmbfhd.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3hkqakfgm.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3xtchzubw.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3mvjvfgse.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3brwtdyws.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3uzwfizux.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3ozpzlmtw.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3htlknvfm.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3nqcpaeey.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3pcjlwddd.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3vspwxmdj.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3ohwpimsg.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3edqrlfma.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3gsuqkqbk.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ezsduuqa.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3ujhaqfpy.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3gvujlfyd.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3bflervbn.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3hexnhyzn.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3ugmenqza.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3ifkbaluc.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3hwvhoytk.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3fkilrybr.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3yueaobwq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3pojbkkqf.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3jylncdbo.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3ktbrebor.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3xnzzzfqb.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3pcqcoicd.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3ffvbpogg.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3cpygukxy.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3iwrzuxew.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ztjyqqqr.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3czgasgqf.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3wwdtforl.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3vbuuhccg.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3lwwfgkqt.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3bjprzyhy.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3qpuukybl.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3uuuiumzs.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3ewfrpkgc.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rfzrhtfj.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3moatoxiz.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3rcwizbhe.html


<!-- 参考信息 -->