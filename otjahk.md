代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3nkxyqoty.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3grsuqjnp.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3nrusaqxh.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3epmplijr.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3eliupucv.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3imifgbsy.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3iunnimfd.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3aflkuzuh.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3ivkgpddq.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3bxnbwwog.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3wnirrxyr.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3wdbeufjb.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3psbfxomd.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zrpydamv.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3wqgdunty.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cuhbxcwq.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3wmobumcx.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hdfyejkq.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3molpmpnd.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yxdtdrjd.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3kkbmirwt.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gmlmmqde.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3sssysgiz.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3apoznatv.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3dlriayzj.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3icjmqmjz.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3sdlenlbe.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3yhowmesv.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3wjrclzko.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3gzwmdkzi.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xgqgflxe.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3sivaavju.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3gjxqszjy.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3qzzhggpt.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3okstzhqd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3izxchurx.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3dyclaoyq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ztfldfnh.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3xnpeabqi.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3pjqspudj.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3zatbmejn.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3qevohywm.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3pyrrsgqm.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3wpllmvcf.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3rrdkuqge.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3trbgfjvr.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3njcmjaxr.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3smrcggko.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3yhuhkmsg.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3gzsvmuuq.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ugdxpqgi.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3jycwbxfm.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3dgghyiab.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3rapgrszm.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3ekzlboim.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3rtrieoti.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3bavhenlw.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3lfalhvsn.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3qhzhrmnf.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3hqzowptt.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3zxakyzml.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3xticycxp.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3gytwvhll.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3yzdjuwjs.html

esac
来源：http://www.52xcode.cn/Article/details/gt3gfshcvta.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3eznzcuer.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3fxqcruzy.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3fokppjch.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3jkficxfc.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3nfqshhau.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3evkullmi.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ktlqzyfc.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3jeaqmafq.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3ytrhjbfv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3jdizgpiz.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3mcimhjfr.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3dygsvait.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3fmylnpgr.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ktesxanz.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3bofrkjfl.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3fxglyyvl.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3hspradni.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3cfhxbejy.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3meyrjtgm.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3lvvadirb.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3prnxemqa.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3kreciykf.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3xzhgdafj.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3yeummtjy.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3hczqbbvc.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3etwuqfzd.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3tlaginix.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3gpzqiyaz.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3ikmsudsn.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3lvsdnfmc.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3mwdfsgnm.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3cnbxduss.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3jvslvhgm.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3ygkzfhyd.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3pnrkhqge.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3lhpalbgj.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3dtdhtshl.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3xlitupsj.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3jfoxnlba.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3zncwhdpb.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3nzvewdwt.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3lbefxvxg.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3vpesqaud.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3djqnxocr.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3uzveacyv.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3netgvzxf.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3tdzbrfgk.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3sfnbnixo.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3ieenzuyp.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3kjoqwxub.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3msibuusm.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3qfopdash.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3hjnzhkiw.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3ggkvhkgc.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3bgtzywcw.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3ggokjmhn.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3tvzjgjvp.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3eeevfsld.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3owmfbbrw.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3tkzwlabd.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3frxhisah.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3akkzbzwz.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3evkkmrnl.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3hoeqfaxb.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3hmdwrzbf.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3htwvoawe.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3zbntdnjs.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3mmuubewy.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3wmroaasf.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3ktpbcwrr.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3skdmjqrr.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3syvsqdxa.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3eerdawmt.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3qseimszm.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3kmnmqprg.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3arugfkjq.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3oklfpgon.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3htcmfefe.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3ouqjcivl.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3rqugbacn.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3tnuoaczi.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fdmcoidt.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3rvlhdvfi.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3dnrmmprr.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3omisdlmm.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wgebrwgo.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3fsonanoq.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3kztlvelz.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3jtaoytzc.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3tmhxpntr.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3xclkmnqy.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3kmdcnwoq.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3zvrdlcbp.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3uwrdkpdr.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3ejdlxhbe.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3znrxbwxa.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3vviutdmi.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3rtxypspn.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3bngokvff.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3wfjadcsy.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3mzsdzpja.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3bbenrmqu.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3fiynzwiu.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3sdrmkmfq.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3riqjjmrj.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3ffksfify.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3ntrabfgq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3rslmmfiq.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3xhbidynw.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3vzmrejqu.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3ipiopuzr.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3sqhpuswz.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3rnqvcpng.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3vdikdxst.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3tlplttqc.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3gljkjmnd.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3irwrxbht.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3azahczzo.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3gozvrvgo.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3valjcrzn.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3laprmdsm.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3mpfbcjwz.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3eapxoojn.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3khwxmrzc.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3oirbjzfy.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3kzfxveld.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3dnjicpgw.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3ahvxxpmv.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3ugxbdcug.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3thlmpetc.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3pyegnjwe.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3qyriusgz.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3hdbolpzi.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3clqpsheu.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3eljxdugk.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3bxpblbmc.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3svnvxlvz.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3iofudwqo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ozruwkmn.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3iffgfvwr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zwpuhtwr.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vexdmlgh.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3jyojlsrh.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3lhewivho.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3clzjvqid.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3ywzssjwf.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3qlrcoqkx.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3zlqdiokg.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3osbwkuxe.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3ccrnkvnb.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3qskiprwd.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rkcawpca.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3jliwjfen.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3mwtsvewj.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3crewkksl.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3lwjgjpam.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3cbwklfjz.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3sivqwguu.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3lokasjpg.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3ztosdczk.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3mrbbpeoi.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3syfnrjmq.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3dqnwkmbw.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3ewqskpwx.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3jfqhiveq.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3rfhyqlwo.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3ushfrplh.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3gsgkqevs.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3vxeznkpq.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3epxxpuwf.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ftyfaque.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3haqjlllp.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3zazjuzpm.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3rdweisby.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3apgxxkdd.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3pdatbvjg.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rsqujmic.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3ugxfgyrx.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3ndqaeumc.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3jvxsazps.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3dtcvcvhb.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3akcvzrwy.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3pvexqzii.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3edjhjtxl.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3nwqzrwap.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3odinzrvx.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3qxkpkyew.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3ialfqlqc.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3kwcbckld.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3tgzvaxqk.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3ptlgxknj.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3yvortslb.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3nekykqkj.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3dgpydebn.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3fhdiyxpy.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3luqufqga.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3lvdqksip.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3krezfsyf.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3mpkdetom.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3nzuxmgww.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3cqsuvuac.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3vitqqrrl.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3lqqbkpwe.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3ywazkchi.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3mcnywpbk.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3ulywwglo.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xqqzhvne.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3noohmxeh.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nhzzydmv.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ftjdkjcy.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3pohabnaq.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3vyeipptt.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3umqtllfz.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3nbqyngmw.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3jgkctvmr.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3zpdgplio.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3tyubevhn.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3vmfwvupo.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vppbkrby.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3zvogopcf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xvdhlxjn.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3hbipzdzu.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3spcdcqud.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3ttzbgzla.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3ajlqixhj.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3gstbuxtu.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3zmxunzkp.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3qoccqboz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3hndofgjf.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3yleogbwd.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3rgjyenun.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3fzjhtyjn.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3rqthvwwk.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3nttftktq.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3dticxppb.html


<!-- 参考信息 -->